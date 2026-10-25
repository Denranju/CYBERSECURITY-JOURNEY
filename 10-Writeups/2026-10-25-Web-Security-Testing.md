# Web Security Testing — Practical Log

**Date:** 25 October 2026

## 1. Objective

To practice inspecting a locally running web application using Kali Linux, curl, Burp Suite, and Nmap, and to learn how to investigate potential web security weaknesses.

## 2. Testing Environment

- **Operating system:** Kali Linux
- **Target:** My local React/Vite service-request application
- **Application URL:** `http://localhost:5173/`
- **Tools:** curl, Burp Suite, Nmap, VS Code

Testing was performed against a local learning application.

## 3. HTTP Response Inspection

### Command

```bash
curl -i http://localhost:5173/
```

### Observation

The application returned `HTTP/1.1 200 OK` and HTML content that referenced the Vite development client and React application files.

### Learning outcome

I learned how to inspect an HTTP response and identify the status code, headers, and response body.

A `200 OK` response confirms that the request succeeded, but does not establish whether the application is secure.

## 4. JavaScript Source Inspection

### Commands

```bash
curl -i http://localhost:5173/src/main.jsx
curl -i http://localhost:5173/src/App.jsx
```

### Observation

The development server returned JavaScript modules and source-map content. The application source referenced components and API functions related to authentication and service requests.

### Security consideration

Exposing source code through a development server warrants a configuration review. This observation alone does not confirm a vulnerability, and production behavior still needs to be assessed.

## 5. Burp Suite

I explored the Proxy and HTTP history features to observe browser requests to the local application.

### Learning outcomes

- HTTP history can help identify endpoints and request methods.
- Request headers and response bodies provide evidence during testing.
- Repeater can be used to modify and resend requests in an authorized environment.

Further request-and-response analysis is still required.

## 6. Nmap

I performed a local IPv6 scan of port 5173.

### Command

```bash
nmap -6 -sT -sV -p 5173 ::1
```

### Observation

Nmap identified port 5173 as open. Its probe received an HTTP 403 response containing a Vite host-allowlist message.

### Interpretation

The response indicates that the development server rejected the particular probe. It is not, by itself, proof of a vulnerability. The development server's host configuration should be reviewed.

## 7. Planned Security Tests

### Authentication

Check whether private resources are accessible when logged out.

### Authorization

Check whether a citizen account is prevented from performing administrator-only actions.

### IDOR/BOLA

Using two test accounts and test records, check whether one citizen can access or modify another citizen's request by changing an object identifier.

### Input validation

Check how the application handles invalid and unexpected input values.

### Configuration

Review the development server configuration and verify that production deployment does not unnecessarily expose development resources.

## 8. Current Findings

- The local application responded successfully to an HTTP request.
- JavaScript modules and source-map content were available through the Vite development server.
- The Nmap probe received a Vite-related HTTP 403 response.
- Authentication and authorization testing remains incomplete.
- No confirmed vulnerability has been established from these observations.

## 9. Lessons Learned

1. HTTP status codes must be interpreted in context.
2. Burp Suite helps investigate application traffic.
3. curl is useful for examining HTTP responses directly from the terminal.
4. Nmap helps identify listening services, but service detection results require interpretation.
5. IDOR/BOLA testing must verify whether unauthorized access or modification actually occurs.
6. Security reports should distinguish observations, hypotheses, and confirmed vulnerabilities.


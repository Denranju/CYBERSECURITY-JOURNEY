# IDOR and BOLA — Web Security Testing

**Date:** 25 October 2026

## 1. Overview

This document records my learning about Insecure Direct Object Reference (IDOR) and Broken Object Level Authorization (BOLA), two important concepts in web application security.

The objective is to understand how to test whether an application correctly restricts access to resources belonging to different users.

## 2. Definitions

### IDOR — Insecure Direct Object Reference

IDOR occurs when an application uses a user-controlled reference, such as a request ID, without properly checking whether the current user is authorized to access the referenced resource.

Example:

```text
GET /api/requests/101
GET /api/requests/102
```

Changing the identifier is not automatically a vulnerability. The security issue exists if the application exposes a resource the user is not authorized to access.

### BOLA — Broken Object Level Authorization

BOLA occurs when an API does not properly enforce authorization for a specific object being accessed or modified.

For example, a citizen should not be able to retrieve or update another citizen's private service request simply by changing its identifier.

## 3. Potential Impact

If confirmed, IDOR/BOLA vulnerabilities may lead to:

- Unauthorized access to private records.
- Exposure of personal or confidential information.
- Unauthorized modification of another user's data.
- Unauthorized deletion of records.

Actual impact depends on the application and the permissions missing from its server-side checks.

## 4. Testing Methodology

I will test only my local application and use test accounts and records that I control.

### Test 1: Access own resource

1. Sign in as Test Citizen A.
2. Open a service request created by Test Citizen A.
3. Capture the relevant API request in Burp Suite.
4. Record the endpoint, HTTP method, request identifier, and response.

**Expected result:** Test Citizen A can access their own authorized request.

### Test 2: Attempt cross-user access

1. Create a separate test request using Test Citizen B.
2. Sign in as Test Citizen A.
3. Replay the relevant request with Test Citizen B's test request identifier.
4. Inspect the response body and server behavior.

**Expected result:** Access is denied unless the application explicitly authorizes that access.

### Test 3: Attempt unauthorized modification

Using a test record, check whether Test Citizen A can change a resource owned by Test Citizen B.

**Expected result:** The server rejects the unauthorized modification and the record remains unchanged.

### Test 4: Verify server-side authorization

Review the API implementation to determine whether the server checks both the authenticated user's identity and their permission to access the requested object.

Hiding buttons in the frontend is not sufficient authorization.

## 5. Tools

- Kali Linux
- Burp Suite Proxy
- Burp Suite Repeater
- curl
- Browser Developer Tools
- VS Code

## 6. Evidence to Record

For each test, record:

- Test account and role.
- HTTP method and endpoint.
- Test resource identifier.
- Relevant request and response.
- Whether unauthorized data was returned or modified.
- Expected versus actual behavior.
- Security impact and recommended remediation.

Do not include real passwords, session tokens, or personal information in published write-ups.

## 7. Remediation

- Enforce object-level authorization on the server for every relevant request.
- Verify that the authenticated user is permitted to access the requested resource.
- Apply role-based permissions where appropriate.
- Validate authorization on read, update, and delete operations.
- Add automated tests for cross-user access attempts.

## 8. Current Status

**Status: Learning and testing in progress.**

I have studied the definitions and testing methodology. I have not yet confirmed an IDOR or BOLA vulnerability in my local application.

A vulnerability should only be reported after reproducible evidence demonstrates unauthorized access or modification.

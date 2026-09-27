# Access Control

Access control vulnerabilities occur when an application does not properly enforce what actions or resources a user is authorized to access.

## 📊 Progress

**Completed: 0 / 13**

| # | Lab | Status | Write-up |
|---:|---|---|---|
| 1 | Unprotected admin functionality | ✅ Completed | [Write-up](./lab-01.md) |
| 2 | Unprotected admin functionality with unpredictable URL | ⬜ | — |
| 3 | User role controlled by request parameter | ⬜ | — |
| 4 | User role can be modified in user profile | ⬜ | — |
| 5 | User ID controlled by request parameter | ⬜ | — |
| 6 | User ID controlled by request parameter, with unpredictable user IDs | ⬜ | — |
| 7 | User ID controlled by request parameter with data leakage in redirect | ⬜ | — |
| 8 | User ID controlled by request parameter with password disclosure | ⬜ | — |
| 9 | Insecure direct object references | ⬜ | — |
| 10 | URL-based access control can be circumvented | ⬜ | — |
| 11 | Method-based access control can be circumvented | ⬜ | — |
| 12 | Multi-step process with no access control on one step | ⬜ | — |
| 13 | Referer-based access control | ⬜ | — |

---

## 🧠 Concepts

### Vertical Privilege Escalation

A lower-privileged user gains access to functionality intended for a higher-privileged user.

### Horizontal Privilege Escalation

A user gains access to resources belonging to another user with the same level of privileges.

### Insecure Direct Object Reference (IDOR)

An application exposes a direct reference to an internal object, such as a user ID or document ID, without properly checking whether the current user is authorized to access it.

### Broken Access Control

The application fails to correctly enforce authorization rules, allowing users to perform actions or access resources they should not be able to access.

---

## 🛠️ Tools

- Burp Suite Professional
- Burp Proxy
- Burp Repeater
- Burp Intruder
- Browser Developer Tools

---

# Lab 01 - Unprotected Admin Functionality

## 🎯 Lab Objective

Access the administrator panel and delete the user `carlos`.

## 🔍 Vulnerability

**Unprotected Admin Functionality**

The application exposes an administrator panel without properly restricting access to authorized administrators.

## 🧪 Steps

### 1.Check `robots.txt`

I accessed:

`/robots.txt`

The response contained:

```text
User-agent: *
Disallow: /administrator-panel
```
This revealed the location of the administrator panel.

### 2.Access the Administrator Panel

I navigated to:

/administrator-panel

The administrator panel was accessible without authentication or authorization.

### 3. Delete the User

The administrator panel contained an option to delete users.

I selected the user carlos and deleted the account.



## 💡 Why It Works

The application does not properly enforce access control on the administrator panel.

Although robots.txt reveals the location of the panel, the main vulnerability is that the administrative functionality can be accessed without proper authorization.

robots.txt is not a security mechanism and should not be relied upon to protect sensitive functionality.

## 🛡️ Remediation

### The application should:

Require authentication for administrative functionality.
Verify that the authenticated user has administrator privileges.
Enforce authorization on every administrative endpoint.
Never rely on hidden URLs as a security mechanism.

## 🧠 What I Learned
robots.txt can reveal interesting application paths.
robots.txt may contain details of disallowed and allowed paths.
Sensitive administrative functionality must have server-side authorization.
Hidden functionality is not necessarily protected functionality.

## 🛠️ Tools
Burp Suite
Web Browser

## ✅ Result
Lab Solved
# Script-Controlled ACL – Restrict Record Access Based on Field Value

## 📌 Project Overview

This project is a ServiceNow Administrator project that demonstrates how Access Control Lists (ACLs) can be used to restrict access to records based on user roles and field values.

The project uses a custom **Institution Details** table containing student information such as roll number, student name, faculty name, branch, email, phone number, and description.

The main focus is to control different record operations such as **READ, CREATE, WRITE, and DELETE** using ServiceNow ACLs.

---

## 🎯 Project Objective

The main objectives of this project are:

- Create users and custom roles in ServiceNow.
- Create a custom Institution Details table.
- Create student records with different branch values.
- Implement role-based access control using ACLs.
- Implement field-based access control for the Branch field.
- Restrict READ access to authorized users.
- Configure CREATE, WRITE, and DELETE ACLs.
- Understand how ServiceNow protects records from unauthorized access.
- Test the implemented access-control rules.

---

## ❗ Problem Statement

In an IT system, different users may require different levels of access to the same information.

If all users are given unrestricted access, unauthorized users may be able to view, create, modify, or delete sensitive records.

Therefore, a mechanism is required to control record access based on the user's role and the value of specific fields.

This project addresses this problem using ServiceNow Access Control Lists.

---

## 💡 Proposed Solution

The proposed solution uses ServiceNow ACLs to control access to the custom Institution Details table.

Different roles are assigned for different operations:

| Role | Operation |
|------|-----------|
| `bb1` | READ |
| `bb2` | CREATE |
| `bb3` | WRITE |
| `bb4` | DELETE |

For READ access, the ACL also evaluates the **Branch** field and restricts access according to the configured EEE branch condition.

Administrators are provided with full access through the ACL script.

---

## 🛠️ Technology Used

- ServiceNow
- ServiceNow Access Control Lists (ACL)
- ServiceNow Advanced ACL Scripting
- JavaScript
- ServiceNow User Administration
- ServiceNow Custom Tables
- ServiceNow Impersonation for Testing

---

# 👥 Users and Roles

## User Created

A test user named:

**EEE User**

was created for validating the access-control configuration.

## Roles Created

The following custom roles were created:

```text
bb1
bb2
bb3
bb4

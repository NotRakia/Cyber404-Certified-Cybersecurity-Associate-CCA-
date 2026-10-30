## 1. While reviewing a classroom exercise, access is assigned through the role payroll-reader. Which model is this?
a. Network address translation

b. Public-key encryption

c. A DNS delegation

d. Role-based access control (this)

## 2. While reviewing a classroom exercise, access depends on department, device posture and time. Which model fits?
a. Static IP routing

b. Disk partitioning

c. Attribute-based access control (this)

d. A checksum

## 3. Use only the permissions table for variant v3. Which identity may read exam-keys?

**The access policy, variant v3** `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| id | identity | resource | read | write |
| :--- | :--- | :--- | :--- | :--- |
| P3-1 | reader-3 | course-notes | true | false |
| P3-2 | editor-3 | course-notes | true | true |
| P3-3 | reader-3 | exam-keys | false | false |
| P3-4 | assessor-3 | exam-keys | true | false |

Answer: assessor-3

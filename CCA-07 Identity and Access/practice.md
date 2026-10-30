## 1. During a junior analyst handover, which pair uses two different authentication factor categories?
a. Password and security key (this)

b. Password and PIN

c. Two different passwords

d. PIN and another memorized phrase

## 2. During a junior analyst handover, which authenticator can provide phishing resistance when properly deployed?
a. Any emailed password reminder

b. A reusable shared password

c. A security question about a pet

d. A verifier-bound cryptographic authenticator such as a passkey (this)

## 3. During a junior analyst handover, which policy is consistent with modern NIST password guidance?
a. Permit known-compromised passwords indefinitely

b. Send passwords in cleartext email

c. Require changes when compromise is suspected or evidenced rather than arbitrary periodic changes alone (this)

d. Require a new password every hour for everyone

Here is the content from the images formatted as text and a Markdown table, suitable for GitHub.

## 4. Use only the permissions table for variant v5. Which identity may write course-notes?
The access policy, variant v5 `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| id | identity | resource | read | write |
| :--- | :--- | :--- | :--- | :--- |
| P5-1 | reader-5 | course-notes | true | false |
| P5-2 | editor-5 | course-notes | true | true |
| P5-3 | reader-5 | exam-keys | false | false |
| P5-4 | assessor-5 | exam-keys | true | false |

Answer: editor-5

## 5. Use only the permissions table for variant v5. Count rows permitting read access specifically to exam-keys. Return an integer.
The access policy, variant v5 `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| id | identity | resource | read | write |
| :--- | :--- | :--- | :--- | :--- |
| P5-1 | reader-5 | course-notes | true | false |
| P5-2 | editor-5 | course-notes | true | true |
| P5-3 | reader-5 | exam-keys | false | false |
| P5-4 | assessor-5 | exam-keys | true | false |

Answer: 1

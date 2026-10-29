## 1. At a small training company, which Windows Security event documents a successful logon?
a. 4624 (this)

b. 4625

c. Sysmon 3

d. Sysmon 11
## 2. At a small training company, which Windows Security event documents a failed logon?
a. 4624 

b. Sysmon 1

c. Sysmon 22

d. 4625 (this)

## 3. At a small training company, in Windows event 4624, what does logon type 3 indicate?
a. Service startup

b. Workstation unlock

c. Network logon (this)

d. Local interactive console logon

## 4. Use only the auth table for variant v1. Which record reports successful logon? Return record_id.

**Authentication, process and response records, variant v1** `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| record_id | time | event_id | account | source | host | logon_type | result | session_id | context | provider | process_guid | image | action | existing_sessions |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| A1-1 | 09:00:00Z | 4625 | learner-1 | 192.0.2.21 | CCA-WS-1 | 3 | failure | . | . | . | . | . | . | . |
| A1-2 | 09:00:20Z | 4625 | learner-1 | 192.0.2.21 | CCA-WS-1 | 3 | failure | . | . | . | . | . | . | . |
| A1-3 | 09:00:40Z | 4625 | learner-1 | 192.0.2.21 | CCA-WS-1 | 3 | failure | . | . | . | . | . | . | . |
| A1-4 | 09:01:00Z | 4624 | learner-1 | 192.0.2.21 | CCA-WS-1 | 10 | success | SESSION-1 | . | . | . | . | . | . |
| A1-5 | 09:01:10Z | 4625 | svc-backup-1 | 10.0.1.9 | CCA-WS-1 | 5 | failure | . | Approved backup job; stored credential not updated after rotation | . | . | . | . | . |
| A1-6 | 09:02:00Z | 1 | learner-1 | . | CCA-WS-1 | . | created | SESSION-1 | . | Sysmon | PROCESS-1 | notepad.exe | . | . |
| A1-7 | 09:03:00Z | . | . | network-events | CCA-WS-1 | . | not_collected | . | Network sensor absent from 09:00:00Z to 09:10:00Z | collection-health | . | . | . | . |
| A1-8 | 09:04:00Z | . | learner-1 | . | . | . | . | . | . | response-record | . | . | account_disabled | not_yet_revoked |

Answer: A1-4

![image](https://github.com/user-attachments/assets/77c17466-7287-4a6f-a9bc-cb2297cba7b7)

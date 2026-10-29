## 1. While reviewing a classroom exercise, in Windows event 4624, which logon type is RemoteInteractive?
a. 3

b. 5

c. 4

d. 10 (this)

## 2. While reviewing a classroom exercise, which Sysmon event type records process creation?
a. 11

b. 22

c. 1

d. 3

## 3. Use only the auth table for variant v3. Which source address is recorded for that successful logon?

**Authentication, process and response records, variant v3** `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| record_id | time | event_id | account | source | host | logon_type | result | session_id | context | provider | process_guid | image | action | existing_sessions |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| A3-1 | 09:00:00Z | 4625 | learner-3 | 192.0.2.23 | CCA-WS-3 | 3 | failure | . | . | . | . | . | . | . |
| A3-2 | 09:00:20Z | 4625 | learner-3 | 192.0.2.23 | CCA-WS-3 | 3 | failure | . | . | . | . | . | . | . |
| A3-3 | 09:00:40Z | 4625 | learner-3 | 192.0.2.23 | CCA-WS-3 | 3 | failure | . | . | . | . | . | . | . |
| A3-4 | 09:01:00Z | 4624 | learner-3 | 192.0.2.23 | CCA-WS-3 | 10 | success | SESSION-3 | . | . | . | . | . | . |
| A3-5 | 09:01:10Z | 4625 | svc-backup-3 | 10.0.3.9 | CCA-WS-3 | 5 | failure | . | Approved backup job; stored credential not updated after rotation | . | . | . | . | . |
| A3-6 | 09:02:00Z | 1 | learner-3 | . | CCA-WS-3 | . | created | SESSION-3 | . | Sysmon | PROCESS-3 | notepad.exe | . | . |
| A3-7 | 09:03:00Z | . | . | network-events | CCA-WS-3 | . | not_collected | . | Network sensor absent from 09:00:00Z to 09:10:00Z | collection-health | . | . | . | . |
| A3-8 | 09:04:00Z | . | learner-3 | . | . | . | . | . | . | response-record | . | . | account_disabled | not_yet_revoked |

**Answer:**
 **192.0.2.23**

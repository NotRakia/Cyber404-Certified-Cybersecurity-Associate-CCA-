## 1. Use only the timeline table for variant v5. Which record records the file read? Return record_id.

**Timeline records, variant v5** `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| record_id | timestamp | action | host | session_id | bytes | source_record |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| T5-1 | 2026-10-20T17:01:00+08:00 | authentication | CCA-WS-5 | SESSION-5 | . | . |
| T5-2 | 2026-10-20T09:02:00Z | process_created | CCA-WS-5 | SESSION-5 | . | . |
| T5-3 | 2026-10-20T09:03:00Z | file_read | CCA-WS-5 | SESSION-5 | 5000 | . |
| T5-4 | 2026-10-20T09:04:00Z | collector_received | CCA-WS-5 | . | . | T5-3 |

Answer: T5-3

## 2. Use only the timeline table for variant v5. Calculate seconds from authentication to file_read after normalizing offsets. Return an integer.

**Timeline records, variant v5** `SYNTHETIC`

Fictional normalized teaching records, not a raw Windows export or a real incident. Each table is a separate exercise unless the lab explicitly joins matching host/session fields. No claim these records describe a real incident.

| record_id | timestamp | action | host | session_id | bytes | source_record |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| T5-1 | 2026-10-20T17:01:00+08:00 | authentication | CCA-WS-5 | SESSION-5 | . | . |
| T5-2 | 2026-10-20T09:02:00Z | process_created | CCA-WS-5 | SESSION-5 | . | . |
| T5-3 | 2026-10-20T09:03:00Z | file_read | CCA-WS-5 | SESSION-5 | 5000 | . |
| T5-4 | 2026-10-20T09:04:00Z | collector_received | CCA-WS-5 | . | . | T5-3 |

Answer: 120

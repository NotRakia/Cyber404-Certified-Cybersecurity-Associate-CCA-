
## 1. During an academy support shift, what does a correctly validated TLS connection primarily protect?
a. The absence of malicious downloads

b. The authorization of every account

c. The channel's confidentiality and integrity with authenticated peer context (this)

d. The truth of every statement on the site

## 2. During an academy support shift, which DNS record type contains an IPv4 address?
a. TXT

b. A (this)

c. AAAA 

d. MX

## 3. Filter variant_id=v2. How many responses returned status 404? 
HTTP requests to a loopback test server, variant v2 `CAPTURED`

Real benign requests recorded by the course's own capture script on 2026-10-23: application logs, not a packet capture. Does not establish malicious activity. Local clock is recorded as observed; no trusted timestamping claim. Rerunning capture changes timestamps, ports, IDs of socket endpoints and downstream release

| record_id | timestamp_utc | method | path | status | client_ip | client_port | server_ip | server_port | declared_content_length | response_body_bytes | client_observed_status | client_observed_body_bytes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| HTTP-V2-1 | 2026-10-23T10:37:52.081Z | GET | /edition-2.txt | 200 | 127.0.0.1 | 55627 | 127.0.0.1 | 55626 | 48 | 48 | 200 | 48 |
| HTTP-V2-2 | 2026-10-23T10:37:52.082Z | GET | /missing-2 | 404 | 127.0.0.1 | 55628 | 127.0.0.1 | 55626 | 8 | 8 | 404 | 8 |
| HTTP-V2-3 | 2026-10-23T10:37:52.084Z | HEAD | /edition-2.txt | 200 | 127.0.0.1 | 55629 | 127.0.0.1 | 55626 | 48 | 0 | 200 | 0 |
| HTTP-V2-4 | 2026-10-23T10:37:52.085Z | POST | /edition-2.txt | 405 | 127.0.0.1 | 55630 | 127.0.0.1 | 55626 | 19 | 19 | 405 | 19 |
| HTTP-V2-5 | 2026-10-23T10:37:52.086Z | GET | /edition-2.txt | 200 | 127.0.0.1 | 55631 | 127.0.0.1 | 55626 | 48 | 48 | 200 | 48 |
| HTTP-V2-6 | 2026-10-23T10:37:52.087Z | GET | /absent-2 | 404 | 127.0.0.1 | 55632 | 127.0.0.1 | 55626 | 8 | 8 | 404 | 8 |

Answer: 2

## 4. Filter variant_id=v2. Sum client-observed body bytes for GET responses with status 200. Return an integer.
HTTP requests to a loopback test server, variant v2 `CAPTURED`

Real benign requests recorded by the course's own capture script on 2026-10-23: application logs, not a packet capture. Does not establish malicious activity. Local clock is recorded as observed; no trusted timestamping claim. Rerunning capture changes timestamps, ports, IDs of socket endpoints and downstream release hashes.

| record_id | timestamp_utc | method | path | status | client_ip | client_port | server_ip | server_port | declared_content_length | response_body_bytes | client_observed_status | client_observed_body_bytes |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| HTTP-V2-1 | 2026-10-23T10:37:52.081Z | GET | /edition-2.txt | 200 | 127.0.0.1 | 55627 | 127.0.0.1 | 55626 | 48 | 48 | 200 | 48 |
| HTTP-V2-2 | 2026-10-23T10:37:52.082Z | GET | /missing-2 | 404 | 127.0.0.1 | 55628 | 127.0.0.1 | 55626 | 8 | 8 | 404 | 8 |
| HTTP-V2-3 | 2026-10-23T10:37:52.084Z | HEAD | /edition-2.txt | 200 | 127.0.0.1 | 55629 | 127.0.0.1 | 55626 | 48 | 0 | 200 | 0 |
| HTTP-V2-4 | 2026-10-23T10:37:52.085Z | POST | /edition-2.txt | 405 | 127.0.0.1 | 55630 | 127.0.0.1 | 55626 | 19 | 19 | 405 | 19 |
| HTTP-V2-5 | 2026-10-23T10:37:52.086Z | GET | /edition-2.txt | 200 | 127.0.0.1 | 55631 | 127.0.0.1 | 55626 | 48 | 48 | 200 | 48 |
| HTTP-V2-6 | 2026-10-23T10:37:52.087Z | GET | /absent-2 | 404 | 127.0.0.1 | 55632 | 127.0.0.1 | 55626 | 8 | 8 | 404 | 8 |

Answer: 96

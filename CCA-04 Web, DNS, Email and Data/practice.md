## 1. During an academy support shift, a web server returns HTTP 200. What does this establish?
a. The server had no vulnerabilities

b. The request succeeded according to that response's semantics (this)

c. The visitor was a trusted employee

d. The response was encrypted

## 2. During an academy support shift, a request receives HTTP 404. What is a defensible interpretation?
a. The server did not find or disclose a current representation of the target (this)

b. The client necessarily launched an exploit

c. The entire server is offline

d. The password was accepted

## 3. During an academy support shift, how does an ordinary HTTP HEAD response differ from GET?
a. It always returns 404

b. It encrypts the request automatically 

c. It authenticates without credentials

d. It sends no response message content (this)

## 4.   Filter variant_id=v2. How many request records are in this assigned capture?  
HTTP requests to a loopback test server, variant v2  `CAPTURED`
Real benign requests recorded by the course's own capture script on 2026-10-23: application logs, not a packet capture. Does not establish malicious activity. Local clock is recorded as observed; no trusted timestamping claim. Rerunning capture changes timestamps, ports, IDs of socket endpoints and downstream release hashes.

| record_id | timestamp_utc            | method | path           | status | client_ip | client_port | server_ip | server_port | declared_content_length | response_body_bytes | client_observed_status | client_observed_body_bytes |
| :-------- | :----------------------- | :----- | :------------- | :----- | :-------- | :---------- | :-------- | :---------- | :---------------------- | :------------------ | :--------------------- | :------------------------- |
| HTTP-V2-1 | 2026-10-23T10:37:52.081Z | GET    | /edition-2.txt | 200    | 127.0.0.1 | 55627       | 127.0.0.1 | 55626       | 48                      | 48                  | 200                    | 48                         |
| HTTP-V2-2 | 2026-10-23T10:37:52.082Z | GET    | /missing-2     | 404    | 127.0.0.1 | 55628       | 127.0.0.1 | 55626       | 8                       | 8                   | 404                    | 8                          |
| HTTP-V2-3 | 2026-10-23T10:37:52.084Z | HEAD   | /edition-2.txt | 200    | 127.0.0.1 | 55629       | 127.0.0.1 | 55626       | 48                      | 0                   | 200                    | 0                          |
| HTTP-V2-4 | 2026-10-23T10:37:52.085Z | POST   | /edition-2.txt | 405    | 127.0.0.1 | 55630       | 127.0.0.1 | 55626       | 19                      | 19                  | 405                    | 19                         |
| HTTP-V2-5 | 2026-10-23T10:37:52.086Z | GET    | /edition-2.txt | 200    | 127.0.0.1 | 55631       | 127.0.0.1 | 55626       | 48                      | 48                  | 200                    | 48                         |
| HTTP-V2-6 | 2026-10-23T10:37:52.087Z | GET    | /absent-2      | 404    | 127.0.0.1 | 55632       | 127.0.0.1 | 55626       | 8                       | 8                   | 404                    | 8                          |

Answer: 6

## 5.  Filter variant_id=v2. Count all responses with status >= 400. Return an integer.

| record_id | timestamp_utc            | method | path           | status | client_ip | client_port | server_ip | server_port | declared_content_length | response_body_bytes | client_observed_status | client_observed_body_bytes |
| :-------- | :----------------------- | :----- | :------------- | :----- | :-------- | :---------- | :-------- | :---------- | :---------------------- | :------------------ | :--------------------- | :------------------------- |
| HTTP-V2-1 | 2026-10-23T10:37:52.081Z | GET    | /edition-2.txt | 200    | 127.0.0.1 | 55627       | 127.0.0.1 | 55626       | 48                      | 48                  | 200                    | 48                         |
| HTTP-V2-2 | 2026-10-23T10:37:52.082Z | GET    | /missing-2     | 404    | 127.0.0.1 | 55628       | 127.0.0.1 | 55626       | 8                       | 8                   | 404                    | 8                          |
| HTTP-V2-3 | 2026-10-23T10:37:52.084Z | HEAD   | /edition-2.txt | 200    | 127.0.0.1 | 55629       | 127.0.0.1 | 55626       | 48                      | 0                   | 200                    | 0                          |
| HTTP-V2-4 | 2026-10-23T10:37:52.085Z | POST   | /edition-2.txt | 405    | 127.0.0.1 | 55630       | 127.0.0.1 | 55626       | 19                      | 19                  | 405                    | 19                         |
| HTTP-V2-5 | 2026-10-23T10:37:52.086Z | GET    | /edition-2.txt | 200    | 127.0.0.1 | 55631       | 127.0.0.1 | 55626       | 48                      | 48                  | 200                    | 48                         |
| HTTP-V2-6 | 2026-10-23T10:37:52.087Z | GET    | /absent-2      | 404    | 127.0.0.1 | 55632       | 127.0.0.1 | 55626       | 8                       | 8                   | 404                    | 8                          |

Answer: 3

![image](https://github.com/user-attachments/assets/6073b457-c29f-4d30-814f-c012e29592f3)


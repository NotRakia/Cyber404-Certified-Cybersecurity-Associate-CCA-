![image](https://github.com/user-attachments/assets/0a465d83-6d8e-4d7f-b9ac-2023bef92b03)


## 1. Convert the authentication timestamp to UTC. Give it as YYYY-MM-DDTHH:MM:SSZ.
### Let's try `ls -la`
![image](https://github.com/user-attachments/assets/25fd616d-a1c5-466f-92a6-aca98c5de8d7)

### Let's see inside uing `cat`
![image](https://github.com/user-attachments/assets/6406b75c-91a1-4cca-94cc-928449f0bd67)\
![image](https://github.com/user-attachments/assets/aac16662-49eb-4a8b-b8df-2328d7fdde86)


Answer: 2026-10-20T09:01:00Z

## 2. How many seconds after the file-read source event was it received by the collector? Return an integer.
Answer: 60

## 3. Which session_id joins the authentication, process and file-read records? Give it exactly.
Answer: SESSION-2

## 4. Which record has the explicit stale backup-credential context? Give the record_id exactly as it appears, for example A1-4.
Answer: A2-5

## 5. Which record documents the known logging limitation? Give the record_id exactly as it appears, for example A1-4.
Answer: A2-7

## 6. Does closeness in time prove that all of this activity was malicious? Answer yes or no.
Answer: no

## 7. Which timeline record shows the file read? Give its record_id.
Answer: T2-3

## 8. Does a file read alone prove transfer to an external destination? Answer yes or no.
Answer: no

## 9. Which session should a proportionate containment step revoke? Give its session_id.
Answer: SESSION-2

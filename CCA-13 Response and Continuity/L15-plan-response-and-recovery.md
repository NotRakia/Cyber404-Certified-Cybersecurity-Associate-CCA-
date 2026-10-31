![image](https://github.com/user-attachments/assets/045bda80-aa0a-41a0-afe5-46d622bf39fc)

## 1. What response action does the response record show? Give the action value exactly.
### Let's try `ls -la`
![image](https://github.com/user-attachments/assets/6b5bde5a-fc25-4032-8f15-c2f45e24fdec)

### Let's see inside uing `cat`
![image](https://github.com/user-attachments/assets/43d60454-9b32-4797-87d3-ed3bbd437757)

![image](https://github.com/user-attachments/assets/876ca07e-74e1-4d35-a939-779dbe93b0e4)


Answer: account_disabled

## 2. What is the recorded state of the existing sessions? Give the value exactly.
Answer: not_yet_revoked

## 3. Which objective states the maximum tolerable data loss as time: RTO or RPO?
Answer: RPO

RPO (Recovery Point Objective) is specifically defined as the maximum acceptable amount of data loss, measured in time. It answers the question: "How much data (in hours, minutes, or seconds) can we afford to lose if a system goes down?" It determines how frequently you need to back up your data. For example, if your RPO is 1 hour, you must back up your data at least every hour so you never lose more than 60 minutes' worth of work.

RTO (Recovery Time Objective) is about downtime, not data loss. It is the maximum acceptable amount of time it takes to restore a system and get it back online after a failure. It answers the question: "How quickly must we get this system working again?"

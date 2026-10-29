![image](https://github.com/user-attachments/assets/49db2e46-ff02-49a4-828e-e43bf5e93c57)

## 1. report.txt has mode rw-r----. Which class may write it: owner, group or others?
Answer: owner
### Let's use `ls` to see files, also use `ls -la` to see all.
![image](https://github.com/user-attachments/assets/43943489-ce0e-4962-aa80-3c4c9a0640cb)

### Let's try to open it using `cat`.
![image](https://github.com/user-attachments/assets/85f9b367-05fd-48ff-bca9-a620c7aea822)

## 2. run.sh has mode rwxr-x---. How many of the three classes (owner, group, others) may execute it. Return an integer?
Answer: 2 (only the owner and group)

## 3. To answer these, should you change permissions on the live system? Answer yes or no.
Answer: no



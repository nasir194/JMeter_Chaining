## Summary
- Here I have performed API Chaining (JMeter Collection) on the DMoney website Transaction APIs .
- I have taken data from CSV files and Run Multiple APIs at a time using 3 Threads group in Jmeter and generate HTML summary report.

### Description
From the dmoney API collection, create JMeter collection (dmoney.jmx) for the following scenario: 

### Scenario:
- 5 agents perform deposits for 10 customers.
- 5 customers send money to another 10 customers.
- 5 customers make payments to 2 merchants.

-> Log in as an admin once and generate a token to use for each of the threads. 
-> Create 3 threads under test plan for each type of transaction and set up agent, customer, and merchant accounts in 3 different CSV files
-> Each thread should have a ramp-up time of 120 seconds.
-> Website for APIs - http://dmoney.roadtocareer.net
  
## How to run?
### Execute the following steps using JMeter:
- ``` git clone <repo_url> ```
- ``` From ApacheJMeter open dmoney.jmx File ```
- ``` Run ```

### Execute the following steps using CLI:
- ``` git clone <repo_url> ```
- ``` jmeter -n -t .\dmoney.jmx -l .\dmoney.jtl -e -o Reports ```

## Generated HTML report for DMoney Jmeter Collection Test
<img width="1141" height="541" alt="Dmoney" src="https://github.com/user-attachments/assets/84fc1058-7551-4033-9d44-c4da28c6b31b" />

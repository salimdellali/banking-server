# banking-server

## User stories

```
Client User Story:
- As a client, I want to create a new bank account using my credentials
- As a client, I want to enter my credentials to be able to connect securely to my bank account
- As a client, I want to check my bank accounts’ balance
- As a client, I want to inject money into my bank account
- As a client, I want to retrieve money from my bank account
- As a client, I want to transfer money to another client
- As a client, I want to see the logs of my transactions
- As a client, I want to be able to delete my bank account

Admin User Story:
- As an admin, I want to be able to check any clients’ bank account
- As an admin, I want to be able to see transactions logs of any clients’ bank account
- As an admin, I want to be able to transfer money from any clients bank account into another
- As an admin, when a client decides to delete his bank account, I want to archive his bank account

System Constraints:
- A balance cannot be less than 0
- A transaction should be ACID
- A cron job is run to deduct a subscription for the bank services fee from all bank accounts periodically
    - The period: can be configured by the admins (e.g: 1 month)
    - The fee amount: can be configured by the admins (e.g: 0.5$)
```

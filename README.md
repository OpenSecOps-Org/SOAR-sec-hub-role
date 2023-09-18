This template is used to se up the role SecurityHubRole in all accounts. It's used by
the Security Hub automation flows to access member accounts as an admin. This
is used for data collection purposes and for remediation purposes.

This will be deployed as a StackSet in the organisational account, in the main region,
to all accounts in the same region.

It will also be deployed as a single stack in the organisational account, in the main region.


## Deployment

First make sure that your SSO setup is configured with a default profile giving you AWSAdministratorAccess
to your AWS Organizations administrative account. This is necessary as the AWS cross-account role used 
during deployment only can be assumed from that account.

```console
aws sso login
```

Then type:

```console
./deploy
```

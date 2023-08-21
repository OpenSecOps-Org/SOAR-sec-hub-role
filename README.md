This template is used to se up the role SecurityHubRole in all accounts. It's used by
the Security Hub automation flows to access member accounts as an admin. This
is used for data collection purposes and for remediation purposes.

This will be deployed as a StackSet in the organisational account, in the main region,
to all accounts in the same region.

It will also be deployed as a single stack in the organisational account, in the main region.

## Deployment

First log in to your AWS organisation using SSO and a profile that gives you
AWSAdministratorAccess to the AWS Organizations admin account.

```console
aws sso login --profile <profile-name>
```

Then type:

```console
./deploy
```

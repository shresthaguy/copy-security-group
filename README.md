# copy-security-group
Import and Export Security Group to different regions VPC

There is no one-click solution to import and export security group from one VPC to other VPC in different regions of same/different account. This requires AWS-cli and jq.

In order to export security group to different account, aws cli must be configured with multiple profiles with credentials of different account.

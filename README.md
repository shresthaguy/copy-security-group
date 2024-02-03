# Copy Security Group to different VPC

Copy/Import and Export Security Group to different VPC of different regions of same/different account. 

There is no one-click solution to import and export security group from one VPC to other VPC in different regions of same/different account. Therefore, I've created a simple script using aws-cli. You must have jq installed for this script to work.

NOTE: In order to export security group to different account, aws cli must be configured with multiple profiles with credentials of different account.

References:
[+] describe-security-groups: https://docs.aws.amazon.com/cli/latest/reference/ec2/describe-security-groups.html
[+] create-security-group: https://docs.aws.amazon.com/cli/latest/reference/ec2/create-security-group.html
[+] revoke-security-group-egress: https://docs.aws.amazon.com/cli/latest/reference/ec2/revoke-security-group-egress.html
[+] authorize-security-group-ingress: https://docs.aws.amazon.com/cli/latest/reference/ec2/authorize-security-group-ingress.html
[+] authorize-security-group-egress: https://docs.aws.amazon.com/cli/latest/reference/ec2/authorize-security-group-egress.html
[+] Install or update the latest version of the AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
[+] Configure AWS CLI: https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-files.html

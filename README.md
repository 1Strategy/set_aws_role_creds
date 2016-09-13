# set_iam_role_creds

## Problem
Terraform doesn't support assuming an AWS IAM role until
a new version is released with this PR included:
[provider/aws: Add support for AssumeRole prior to operations](https://github.com/hashicorp/terraform/pull/8638).

## Solution
This bash script assumes you have a master IAM user with an `AccessKeyId` and
`SecretAccessKey` defined in ~/.aws/credentials.

## Usage
You will need to set the `user` and `profile` variables in the bash script to use it.

## License
Apache 2.0

# s3build

s3build is a simple bash script to build a new s3 bucket with dedicated access and secret keys.
It use the aws command to create amazon services resources and jq utility to parse json results.

## Prerequistes

* `aws`
  Properly configured with an access id allowing creation of IAM users, policies and s3 resources.
  See [http://aws.amazon.com/cli/](http://aws.amazon.com/cli/) to install and configure.
* `jq`
  `apt-get install jq` on Debian/Ubuntu

## Usage

```
$> ./s3build
Creating user 'XXXXXXXXXXXXXXXXXXXXXX'... done.
Creating new access and secret key... done.
Creating new bucket... done.
Generating user policy... done.

URL: s3://AWS_ACCESS_KEY_ID:AWS_SECRET_ACCESS_KEY@S3_BUCKET

```

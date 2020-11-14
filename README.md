# Learn LocalStack
Notes on how to use [localstack](https://localstack.cloud/) in development.

## Getting Started

First its very easy to run localstack as there is a docker image, with:

``` {bash}
curl -o docker-compose.yml https://raw.githubusercontent.com/localstack/localstack/master/docker-compose.yml
docker-compose up
```

Next, set up the [aws-cli](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html)

Test with:

``` {bash}
alias awslocal="aws --endpoint-url http://localhost:4566"
awslocal s3 ls
awslocal s3 mb s3://mybucket
awslocal s3 cp README.md s3://mybucket
awslocal s3 ls s3://mybucket
```

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
aws s3 ls --endpoint https://localhost:4566
```

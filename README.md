# mock-server-account-service-api
This is a mock service for the account service API to be used by other projects where the account service is used as a dependency.


## Pre-Requisites:

1. Docker
2. docker-compose
3. Make sure your docker daemon is up and running

# Follow the steps below to run it locally

## Step 1: Spinning up the container with mock-server

`docker-compose up`

## Step 2: Sending requests

`curl localhost:1080/api/v1/ad-account/2`

You should get the mocked response which is this:

`{
  "id" : 2,
  "customerId" : 12343336,
  "type" : 1,
  "clientId" : 4562229,
  "token" : "xxxxxxxxxxxxxxxxxxxxx",
  "oAuthToken" : "xxxxxxxxxxxxxxxxx",
  "isSandbox" : false,
  "publisherNetwork" : 0,
  "marketId" : 61
}`

This is still a work in progress and more details will be added as updates are being done, thanks.

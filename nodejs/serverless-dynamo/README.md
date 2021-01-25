# About

This is an example repository that demonstrates auto-instrumenting a nodeJS/dynamo/serverless framework application with Epsagon

# What it Does

This reposititory will use serverless framework to deploy 5 new lambda functions to the region specified. It will also create a dynamoDB table (default name serverless-dynamo). The 5 lambda functions will be auto-instrumented (via serverless plugin) to send traces into your Epsagon account.

# Prerequisites

- Serverless CLI (npm install -g serverless)
- AWS Account, CLI

# Installation

- Clone repo, switch to nodejs/serverless-dynamo/ directory
- `npm install`
- add your epsagon token to serverless.yml
- optional: update aws region in serverless.yml (default: us-east-1)
- `serverless deploy`

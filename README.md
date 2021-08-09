# Example of Serverless Next.js with AWS CDK

## Getting started

```bash
$ yarn create next-app --example https://github.com/hideokamoto/serverless-nextjs-cdk-example
```

## Local development

You can run the Next.js application by the command.

```bash
$ yarn dev
```

## Deploy to AWS

We need to build the CDK stack before running the deployment command.

```bash
$ yarn build
```

Then, run the CDK command.
It will build the Next.js application automatically.
So you don't have to run the `next build` command.

```bash
$ yarn cdk deploy
```

## Contributing
### Getting started

```bash
$ git clone git@github.com:hideokamoto/serverless-nextjs-cdk-example.git
$ cd serverless-nextjs-cdk-example
$ yarn
$ yarn cdk bootstrap
```

### Local development (Next.js)

```bash
$ yarn dev
```

## Build

```bash
# AWS CDK stack
$ yarn build

# Next.js
# If you want to deploy using serverless-nextjs, do not use it.
$ yarn next:build
```


## [Appendix][AWS CDK] Welcome to your CDK TypeScript project!

This is a blank project for TypeScript development with CDK.

The `cdk.json` file tells the CDK Toolkit how to execute your app.

### Useful commands

 * `npm run build`   compile typescript to js
 * `npm run watch`   watch for changes and compile
 * `npm run test`    perform the jest unit tests
 * `cdk deploy`      deploy this stack to your default AWS account/region
 * `cdk diff`        compare deployed stack with current state
 * `cdk synth`       emits the synthesized CloudFormation template

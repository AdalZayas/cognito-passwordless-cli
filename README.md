# Cognito Cli passwordless login
A cli to interact with your cognito user pool, create accounts, login, verify phone number, verify email, etc.

## Installation

Install using yarn

```
yarn global add cognito-passwordless-cli
```

Install using npm

```
npm i -g cognito-passwordless-cli
```
## Documentation

### Help

To get a list of commands and usage hints use

```
cognito-cli --help
```

### Commands

#### createConfig

    Create the config that will be used to perform various cognito functions

    Config 
    cognito-cli createConfig --region=us-east-1  --userPoolId=123 --userPoolWebClientId=123 --email=numberPhone

#### getConfig

    Get the current configuration that will be used to perform various cognito functions
    
    Example
    cognito-cli getConfig


> For one off changes you can pass config args to any command. For example: cognito-cli signin --email=mac@wednesday.is --userPoolId=123


#### signin

    Use the current config to sign in and get tokens
    
    Example
    cognito-cli signin

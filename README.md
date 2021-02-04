# Cognito Cli

## Documentation

### Help

To get a list of commands and usage hints use

```
cognito-cli --help
```

### Commands

#### createConfig

    Create the config that will be used to perform various cognito functions

    Example
    cognito-cli createConfig --region=us-east-1 --givenName=mac \
        --lastName=mac --userPoolId=123 --userPoolWebClientId=123 \
        --mfaEnabled=true --email=mac@wednesday.is --password=123 \
        --phoneNumber=+10101001 --emailVerified=true --phoneVerified=false

#### getConfig

    Get the current configuration that will be used to perform various cognito functions
    
    Example
    cognito-cli getConfig

#### signin

    Use the config to get to sign in and get tokens
    
    Example
    cognito-cli signin

#### signup

    Use the current config to create a new user
    
    Example
    cognito-cli signup
    
    
#### verifyEmail

    Verify the email in the config. 
    
    Example
    cognito-cli verifyEmail

    
    
#### verifyPhone

    Verify the phone in the config. 
    
    Example
    cognito-cli verifyPhone
    
    
#### forceVerify

    Force verify email, phone number attributes in cognito 
    
    Example
    cognito-cli forceVerify
    
    
#### updateAttributes

    Update the congito attributes. 
    
    Example
    cognito-cli updateAttributes

#### enableMFA

    Enable MFA for the user.  
    
    Example
    cognito-cli enableMFA


For one off changes you can pass config args to any command. 

Example

cognito-cli signin --email=mac@wednesday.is --userPoolId=123
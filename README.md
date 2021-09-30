# aws-sam


## Build
To the application you'll need to run the following command
1. follow to project root directory
```
sam build
```
## Local setup
in order to test the functionality locally, you will to install _docker_ before using the below command
```
sam local start-api
```
### guided
For first time deployment we will need to use guided flag in order to setup the proper configurations of the stack
```
sam deploy --guided
```
### production deployment
Once you have initiated the guided settings, a file titled `.aws-sam` will appear on top of your project directory root.
You should be adding this folder to ignore as it has environment specific configurations.
Then you can use the following command to provision all the necessary resources and deploy your function
```
sam deploy
```
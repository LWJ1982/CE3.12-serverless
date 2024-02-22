# CE3.12-serverless

## Update 01 - update github with README.md
- update README.md
## Update 02 - install serverless
terminal 
- nvm install lts 
- npm install -g serverless
check installation 
- serverless -v or sls -v
a. create json file
- npm init
b. create json file (alternate)
- serverless

New files
- index.js
- serverless.yml

## update 03 - update serverless.yml with configuration
- npm install serverless
- npm install serverless-offline --save-dev

run serverless
- sls offline start or - serverless offline
### code to change port 
- sls offline start --httpPort 3003

## update 04 - deploy
- serverless deploy or sls deploy

## update 05 - add unit testing
- npm install --save-dev jest
- npm install --save-dev jest -g <for global>
New file
- index.test.js
- update package.json 
    - under scripts : 
    remove -> "test": "echo \"Error: no test specified\" && exit 1"
    replace -> "test": "jest"
- update index.js
   -under body:JSON below message
    remove -> input: event

## update 06 -del 
- sls remove

## update 07 - update CICD github workflow
New file
- main.yml
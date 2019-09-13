# Sample NodeJS application for GitHub Actions 

Sample workflow to build and deploy node js app. 

### Links:

sample aws action usage - v1 workflow: https://gist.github.com/pahud/4bdc6cde7b55c4fb8bd8c886dd57787e


use aws cli instead of eb cli: https://stackoverflow.com/questions/37644881/how-to-use-aws-cli-with-elastic-beanstalk


aws actions:
1. Actions related to amazon eks (amazon elastic container service for kubernetes): https://github.com/actions/aws/tree/master/kubectl
2. Action for aws cli: https://github.com/actions/aws/tree/master/cli
3. 


Github action syntax: https://help.github.com/en/articles/workflow-syntax-for-github-actions
                        https://help.github.com/en/articles/metadata-syntax-for-github-actions



github secrets doc:
https://help.github.com/en/articles/virtual-environments-for-github-actions#creating-and-using-secrets-encrypted-variables

softwares installed in github agents: https://help.github.com/en/articles/software-in-virtual-environments-for-github-actions


ebs commands: https://docs.aws.amazon.com/cli/latest/reference/elasticbeanstalk/index.html

managing beanstalk applications: https://docs.aws.amazon.com/elasticbeanstalk/latest/dg/applications.html




Running commands:
aws elasticbeanstalk create-application-version --application-name rai-demo --version-label v0.1 --description MyAppv1 --source-bundle S3Bucket="rai-demo-bucket",S3Key="NodeExpressSampleApp.1.zip"
aws elasticbeanstalk update-environment --application-name rai-demo --environment-name raiDemo-env --version-label v0.1

App: rai-demo
Env: RaiDemo-env
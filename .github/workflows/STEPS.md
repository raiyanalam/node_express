# Steps:

1. Create an EBS application
2. Create an Environment that will be used in the application
3. Create S3 bucket to store the source code zip file
4. Store the AWS credentials in GitHub Repo(secret section)
4. In the yaml:
    <ul>
    <li>Checkout and Zip the contents</li>
    <li>Copy the zip to s3 bucket </li>
    <li>Create the app for ElasticBeanstalk</li>
    <li>Deploy the app for ElasticBeanstalk</li>
</ul>

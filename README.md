# Cloud Formation Templates

## One-Click Deployments:

1. [S3 Bucket Configured for Static Website Hosting](https://console.aws.amazon.com/cloudformation/home?region=us-east-1#/stacks/new?stackName=staticwebhostbucket&templateURL=https://002-cf-templates.s3.amazonaws.com/public-bucket-web-hosting.yaml) ([Source Code](https://github.com/jamesshapiro/cloud-formation-templates/blob/master/s3-bucket-for-static-website-hosting.yaml))

## Notes:

### s3-bucket-for-static-website-hosting.yaml

Differences from [Creating an Amazon S3 bucket for website hosting and with a DeletionPolicy](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/quickref-s3.html) example:

- Updated to remove default PublicAccessBlockConfiguration settings, which will prevent the website from being publicly accessible. The example from the docs is outdated for this reason.
- Added Default Encryption to bucket.
- No Deletion Policy.
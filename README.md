# aws-cloudformation-ecs-senzing-stack-basic

## Synopsis

The `aws-cloudformation-ecs-senzing-stack-basic` AWS Cloudformation template
deploys Senzing for use with a previously deployed
[aws-cloudformation-database-cluster](https://github.com/Senzing/aws-cloudformation-database-cluster) Cloudformation stack.

## How to deploy without much thinking

1. :warning: **Warning:** This Cloudformation deployment will accrue AWS costs.
   With appropriate permissions, the
   [AWS Cost Explorer](https://aws.amazon.com/aws-cost-management/aws-cost-explorer/)
   can help evaluate costs.
1. Visit [AWS Cloudformation with Senzing template](https://console.aws.amazon.com/cloudformation/home#/stacks/new?stackName=senzing-db&templateURL=https://s3.amazonaws.com/public-read-access/aws-cloudformation-ecs-senzing-stack-basic/cloudformation.yaml)
1. At lower-right, click on "Next" button.
1. In **Specify stack details**
    1. In **Parameters**
        1. In **Security responsibility**
            1. Understand the nature of the security in the deployment.
            1. Once understood, enter "I AGREE".
        1. In **Senzing installation**
            1. Accept the End User License Agreement
        1. In **Security**
            1. Enter your email address.  Example: `me@example.com`
        1. In **Identify existing resources**
            1. Enter the stack name of the previously deployed
               [aws-cloudformation-database-cluster](https://github.com/Senzing/aws-cloudformation-database-cluster)
               Cloudformation stack
    1. Other parameters are optional.
       The default values are fine.
    1. At lower-right, click "Next" button.
1. In **Configure stack options**
    1. At lower-right, click "Next" button.
1. In **Review senzing-poc**
    1. Near the bottom, in **Capabilities**
        1. Check ":ballot_box_with_check: I acknowledge that AWS CloudFormation might create IAM resources."
    1. At lower-right, click "Create stack" button.

## A Hack

Unfortunately, the AWS Cloudformation template does not support a particular parameter for the AWS Aurora Postgres Serverless database
that is needed in this stack.
To work around this limitation, see
[How to set AWS RDS force-scaling-capacity](https://github.com/Senzing/knowledge-base/blob/master/HOWTO/set-aws-rds-force-scaling-capacity.md).
If possible, add a "thumbs" up to
[AWS Cloudformation issue #298](https://github.com/aws-cloudformation/aws-cloudformation-coverage-roadmap/issues/298)
to draw attention to this AWS Cloudformation defect.

## Additional topics

1. [How to load AWS Cloudformation queue](https://github.com/Senzing/knowledge-base/blob/master/HOWTO/load-aws-cloudformation-queue.md)
1. [How to update Senzing license](https://github.com/Senzing/knowledge-base/blob/master/HOWTO/update-senzing-license.md)

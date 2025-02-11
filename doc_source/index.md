# AWS Secrets Manager User Guide

-----
*****Copyright &copy; Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What is AWS Secrets Manager?](intro.md)
   + [Compliance with standards](asm_compliance.md)
   + [Support and feedback for AWS Secrets Manager](support-and-feedback.md)
+ [Get started with AWS Secrets Manager](getting-started.md)
+ [AWS Secrets Manager tutorials](tutorials.md)
   + [Tutorial: Create and retrieve a secret](tutorials_basic.md)
   + [Tutorial: Rotate a secret for an AWS database](tutorials_db-rotate.md)
   + [Tutorial: Rotate a user secret with a master secret](tutorials_db-rotate-master.md)
+ [Secrets Manager best practices](best-practices.md)
+ [Authentication and access control for AWS Secrets Manager](auth-and-access.md)
   + [Attach a permissions policy to an identity](auth-and-access_iam-policies.md)
   + [Attach a permissions policy to a secret](auth-and-access_resource-policies.md)
   + [AWS managed policies available for use with AWS Secrets Manager](reference_available-policies.md)
   + [Determine who has permissions to your secrets](determine-acccess_examine-iam-policies.md)
   + [Permissions for users in a different account](auth-and-access_examples_cross.md)
   + [Permissions policy examples](auth-and-access_examples.md)
   + [Permissions reference for Secrets Manager](reference_iam-permissions.md)
+ [Create and manage secrets with AWS Secrets Manager](managing-secrets.md)
   + [Create a secret](manage_create-basic-secret.md)
   + [Protect additional sensitive information](manage_what-not-to-put-in-secret-text.md)
   + [Modify a secret](manage_update-secret.md)
   + [Enhanced search capabilities for secrets in Secrets Manager](manage_search-secret.md)
   + [Delete a secret](manage_delete-secret.md)
   + [Restore a secret](manage_restore-secret.md)
   + [Create and manage multi-Region Secrets Manager secrets](create-manage-multi-region-secrets.md)
      + [Configure primary and replica secrets](multi-region-config.md)
         + [Retry secret replication](retry-replica.md)
         + [Create a replica secret from an existing secret](replicate-existing-secret.md)
      + [Manage multi-Region secrets in Secrets Manager](manage-multiregion-secret.md)
         + [Delete a replica secret](delete-replica.md)
         + [Edit an encryption key](edit-key.md)
         + [Add additional Regions to a replica secret](add-regions.md)
         + [Rotate multi-Region secrets](rotate-replica.md)
         + [Promote a replica secret to a standalone secret](standalone-secret.md)
         + [Find multi-Region secrets](search-multiregion-secret.md)
   + [Automate secret creation in AWS CloudFormation](integrating_cloudformation.md)
   + [Tag your secrets](managing-secrets_tagging.md)
+ [Retrieve secrets](retrieving-secrets.md)
   + [Cache secrets to improve performance](use-client-side-caching.md)
+ [Rotate your AWS Secrets Manager secrets](rotating-secrets.md)
   + [Rotation strategies](rotating-secrets_strategies.md)
   + [Automatically rotate an Amazon RDS, Amazon DocumentDB, or Amazon Redshift secret](rotate-secrets_turn-on-for-db.md)
   + [Automatically rotate another type of secret](rotate-secrets_turn-on-for-other.md)
   + [Rotate a secret now](rotate-secrets_now.md)
   + [How rotation works](rotate-secrets_how.md)
   + [Network access for the rotation function](rotation-network-rqmts.md)
   + [Permissions for the Lambda rotation function](rotating-secrets-required-permissions-function.md)
   + [Customize a Lambda rotation function for Secrets Manager](rotate-secrets_customize.md)
   + [Secrets Manager rotation function templates](reference_available-rotation-templates.md)
+ [Using Secrets Manager with VPC endpoints](vpc-endpoint-overview.md)
   + [Create an endpoint policy for your Secrets Manager VPC endpoint](vpc-endpoint-policy.md)
+ [Monitor the use of your AWS Secrets Manager secrets](monitoring.md)
   + [Monitor Secrets Manager secrets using AWS Config](integrating_awsconfig.md)
      + [AWS Config supported rules for Secrets Manager](aws-config-rules.md)
         + [AWS Config supported resources for Secrets Manager](aws-config-resources.md)
      + [Best practices using AWS Config](implementing-awsconfig-rules.md)
      + [Configure AWS Config Secrets Manager rules](configuring-awsconfig-rules.md)
         + [View Secrets Manager rules in AWS Config](view-secrets-config.md)
      + [Configure AWS Config Multi-Account Multi-Region Data Aggregator for secrets management best practices](configure-awsconfig-aggregator.md)
+ [AWS services integrated with AWS Secrets Manager](integrating.md)
   + [Store AWS CodeBuild registry credentials with Secrets Manager](integrating-codebuild.md)
   + [Integrate Secrets Manager with Amazon Elastic Container Service](integrating-ecs.md)
   + [Store Amazon EMR registry credentials with Secrets Manager](integrating-emr.md)
   + [Integrate Secrets Manager with AWS Fargate](integrating-fargate.md)
   + [Integrate Secrets Manager with AWS IoT Greengrass](integrating-greengrass.md)
   + [Use Secrets Manager secrets in Amazon Elastic Kubernetes Service](integrating_csi_driver.md)
      + [Tutorial: Create and mount a secret in an Amazon EKS pod](integrating_csi_driver_tutorial.md)
   + [Retrieving your secrets with the Parameter Store APIs](integrating_parameterstore.md)
   + [Managing SageMaker repository credentials with Secrets Manager](integrating-sagemaker.md)
   + [Using Security Hub for security best practices in Secrets Manager](integrating-securityhub.md)
   + [Running everything in a VPC](integrating_vpc.md)
   + [Integrating Zelkova with Secrets Manager resource policies](integrating-zelkova.md)
+ [Security in AWS Secrets Manager](security.md)
   + [Mitigate the risks of using the AWS CLI to store your secrets](security_cli-exposure-risks.md)
   + [Data protection in AWS Secrets Manager](data-protection.md)
   + [Secret encryption and decryption](security-encryption.md)
   + [Infrastructure security in AWS Secrets Manager](infrastructure-security.md)
   + [Resiliency in AWS Secrets Manager](disaster-recovery-resiliency.md)
   + [Compliance validation for AWS Secrets Manager](secretsmanager-compliance.md)
+ [Troubleshoot AWS Secrets Manager](troubleshoot.md)
   + [Troubleshoot general issues](troubleshoot_general.md)
   + [Troubleshoot AWS Secrets Manager rotation of secrets](troubleshoot_rotation.md)
+ [Call the API by sending HTTPS query requests](query-requests.md)
+ [AWS Secrets Manager quotas](reference_limits.md)
   + [Add retries to your application](quotas_throttling.md)
+ [Document history for AWS Secrets Manager](document-history.md)
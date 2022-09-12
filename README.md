A simple CodePipeline for deploying resources like
- Transit Gateway
    
- VPC and subnets
    
- EKS cluster
    
- EKS self managed nodegroup

Notes:
- Each Pipeline will deploy a test environment first - which will require manual approval - and followed by prod environment deployment on the same account. 

- Test environment will be destroyed prior to Prod environment deployment.  

- Each Pipeline will create an S3 bucket for artifact store. Any updates on the artifact (in .zip format) on the S3 bucket will trigger a pipeline run

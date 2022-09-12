A simple CodePipeline for deploying resources like
    - Transit Gateway
    
    - VPC and subnets
    
    - Private EKS cluster
    
    - EKS self managed nodegroup

Each Pipeline will deploy a test environment first - which will require manual approval - and followed by prod environment deployment on the same account. Test environment will be destroyed prior to Prod environment deployment.  


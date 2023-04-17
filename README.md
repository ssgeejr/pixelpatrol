#pixelpatrol
Used to search websites for pixel code

Pre-Steps:
Install Terraform (this will include python and boto3)
Ask your admin to provide you with AWS Key/Secret
In your home directory, create the folder: .aws

Inside that directory create two files, the first is 'config' and add something similiar
```
[default]
region = us-east-2
output = json

region = us-east-2
output = json
```

The second file is 'credentials' and add something similiar
```
[default]
aws_access_key_id = ############################
aws_secret_access_key = ######################################

[wmmc]
aws_access_key_id = ############################
aws_secret_access_key = ######################################
```


review the pixelpatrol.tf, then execute the following commands. 

terraform init
terraform validate
terraform apply 
#terraform apply --auto-approve
terraform destroy
#terraform destroy --auto-approve


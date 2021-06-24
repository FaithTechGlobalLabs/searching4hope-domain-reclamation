## How to run terraform scripts directly
**Requires AWS credentials configured**

1. `terraform init`
2. `terraform fmt`
3. `terraform validate`
4. `terraform apply -var"site_domain=YOUR_SITE_DOMAIN"`
5. `terraform destroy`

aws s3 cp website/ s3://$(terraform output -raw website_bucket_name)/ --recursive

## How to run docker image

docker build --build-arg AWS_ACCESS_KEY_ID=<YOUR_ACCESS_KEY> --build-arg AWS_SECRET_ACCESS_KEY=<YOUR_SECRET_KEY> --build-arg DOMAIN_NAME=howtobuyheroin -t s4h_terraform .

https://learn.hashicorp.com/tutorials/terraform/cloudflare-static-website

Need to create a local `example.tvars` file that provides values for variables defined in `variables.tf`

aws s3 cp website/ s3://$(terraform output -raw website_bucket_name)/ --recursive


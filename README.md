# Searching4Hope Domain Reclamation Project

Given a list of domains have been identified and purchased
When the list is dropped in an S3 bucket
Then the list is parsed and a website is created for each domain in the list

Given a website in S3 has been provisioned
When request is made to populate S3 bucket
Then HTML template is populated with appropriate content
And stored in S3 bucket

Given a website in S3 has been provisioned
Then create CNAME record to associated domain name with bucket name

## Technologies

- AWS S3, to store and serve the static website
- Terraform, to automate the creation of the S3 buckets
- Python, to create CName entries in Domain Name Host

## Development Tools

## How to run terraform scripts

1. `cd terraform`
2. `terraform init`
3. `terraform fmt`
4. `terraform validate`
5. `terraform apply -var"site_domain=YOUR_SITE_DOMAIN"`
6. `terraform destroy`

## Reference Materials

- [How to Host a Website on S3 Without Getting Lost in the Sea](https://medium.com/@kyle.galbraith/how-to-host-a-website-on-s3-without-getting-lost-in-the-sea-e2b82aa6cd38)
- [Hosting a static website using Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html)
- [Tutorial: Configuring a static website on Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html)
- [Terraform](https://www.terraform.io/)
- [Terraform Learn: AWS Infrastructure](https://learn.hashicorp.com/tutorials/terraform/aws-build)
- [Terraform AWS Provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)
- [Customize Terraform Configuration with Variables](https://learn.hashicorp.com/tutorials/terraform/variables?in=terraform/configuration-language&utm_source=WEBSITE&utm_medium=WEB_IO&utm_offer=ARTICLE_PAGE&utm_content=DOCS)
- [Set values with a .tfvars file](https://learn.hashicorp.com/tutorials/terraform/sensitive-variables?in=terraform/configuration-language#set-values-with-a-tfvars-file)
- [Set values with environment variables](https://learn.hashicorp.com/tutorials/terraform/sensitive-variables?in=terraform/configuration-language#set-values-with-environment-variables)



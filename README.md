# Searching4Hope Domain Reclamation Project

How might we create a scalable tech-enabled ministry model for Searching4hope to meet the growing needs of an increasingly desperate world?
How can we create a scalable, automated solution for creating websites for domains found and purchased that contain content that points the seekers to a Christ centered message as an alternative for what they were originally looking for.


* See [Issues](https://github.com/coombsj/searching4hope/issues) for future work * 

Companion project: https://github.com/dwinniford/searching4hope-template-generator

## Technologies

* AWS S3, to store and serve the static website
* Terraform, to automate the creation of the S3 buckets
* Python, to create CName entries in Domain Name Host

## Reference Materials

* [How to Host a Website on S3 Without Getting Lost in the Sea](https://medium.com/@kyle.galbraith/how-to-host-a-website-on-s3-without-getting-lost-in-the-sea-e2b82aa6cd38)
* [Hosting a static website using Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html)
* [Tutorial: Configuring a static website on Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/HostingWebsiteOnS3Setup.html)
* [Terraform](https://www.terraform.io/)
* [Terraform Learn: AWS Infrastructure](https://learn.hashicorp.com/tutorials/terraform/aws-build)
* [Terraform AWS Provider](https://registry.terraform.io/providers/hashicorp/aws/latest/docs)
* [Customize Terraform Configuration with Variables](https://learn.hashicorp.com/tutorials/terraform/variables?in=terraform/configuration-language&utm_source=WEBSITE&utm_medium=WEB_IO&utm_offer=ARTICLE_PAGE&utm_content=DOCS)
* [Set values with a .tfvars file](https://learn.hashicorp.com/tutorials/terraform/sensitive-variables?in=terraform/configuration-language#set-values-with-a-tfvars-file)
* [Set values with environment variables](https://learn.hashicorp.com/tutorials/terraform/sensitive-variables?in=terraform/configuration-language#set-values-with-environment-variables)
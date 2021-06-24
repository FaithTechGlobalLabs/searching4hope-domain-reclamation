FROM hashicorp/terraform:light

ENV TF_VAR_site_domain=howtobuyheroin

COPY *.tf ./

RUN terraform init
RUN terraform plan
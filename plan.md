1. A file is dropped into an S3 bucket that then triggers a lambda to process that file. This file will contain a list of domain names.
2. The processor lambda will itterate over the list of domain names, calling a worker process (lambda) for each domain name.
3. This worker process will create the S3 bucket with the right permissions and name based on the domain name passed in
4. When the bucket has finished being created this will trigger another process to generate the HTML content and put that content into the newly created S3 bucket.
5. Another process needs to be kicked off to create a CName entry in the domain name host for this new website, there are examples of scripting this out in Google, but also dependent on which domain name host you are working with.

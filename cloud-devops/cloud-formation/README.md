# udagram

This project contains all the Cloudformation scripts to deploy udagram application

To have a look at the website I deployed, you can click this [link](http://udagr-WebAp-11WPGZDWVC9D1-841361458.us-west-2.elb.amazonaws.com/)

## How to deploy

As a prerequisite, you need to have a network infrastructure. To deploy 
it :

```bash
sh create.sh network network.yml network-parameters.json
```

When you have this, you can deploy the udagram application by doing : 

```bash
sh create.sh udagram final-project-starter.yml final-project-parameters.json
```

When you're done, delete the stack with : 

```bash
aws cloudformation delete-stack --stack-name udagram
```

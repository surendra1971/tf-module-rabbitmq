# tf-module-rabbitmq


```
AMAZON MQ is a managed service offered in AWS for RabbitMQ .

But application is not comptatible with the version provided by AWS Amazon MQ. Hence, we will still stick to creating a VM and install RabbitMQ on the top of it.

```

All the terraform code to provision RabbitMQ will be hosted in this repository.
This will be the backend module, which will be called from the root module "terraform-databases"

### Here is our plan :

```
    * We will create a t3.micro VM in the Private Subnet 1 
    * We will install rabbitMQ on the top of it.
    * Using remote_provisioner, we are going to configure RabbitMQ on the top of the VM.
```
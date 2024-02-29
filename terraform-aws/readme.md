## Terraform AWS EC2 Instance Provisioning

### EC2 Instance Provisioning

1. Navigate to 'environment/dev/ec2' folder, run the command:

```bash 
cd prometheus-stack/
```
2. Open 'ec2.tfvars' file and modify it with your desired details. File contains variables used in terraform configuration. 

### Deployment
1. format terraform code per HCL canonical standards in working dir, run the code:

```bash
terraform fmt
```

2. validate terraform code in working dir:

```bash
terraform validate
```

3. initialize terraform in working dir:
```bash
terraform init
```

4. create an execution plan:

```bash
terraform plan --var-file=../vars/ec2.tfvars
```

5. apply changes to create ec2 instance:
```bash
terraform apply --var-file=../vars/ec2.tfvars
```

6. to destroy the ec2 instance and associated resources:
```bash
terraform destroy --var-file=../vars/ec2.tfvars
```

**note**: always review the execution plan ('terraform plan') before applying changes to avoid unintended modifications

### Terraform command reference
update all outputs:
<pre>terraform refresh</pre>
show all outputs:
<pre>terraform show</pre>
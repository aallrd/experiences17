# Infrastructure as code: model and provision your Azure services with Terraform and Packer

## Terraform

- Versionning infrastructure
- Multi-vendor (Azure, AWS, ...)
- Dry run mode
- Glossary
- - Provider
- - Variable
- - Ressource
- - Argument
- - Attribut
- Graph notion to represent dependencies (terraform graph)
- __SOLARIS !!!__
- Fast release cycle 1/2 weeks

### Configure Terraform with Azure

- Create a Service Principal in the Tenant
- ConnexionAzure.tf
- New resource group rg.tf
- `terraform init`
- `terraform plan`
- `terraform apply`
- Can update exisiting resources
- Can return provider properties when created
- `terraform destroy` -> clean what you just deployed

## Packer

- Create images
- Glossary:
- - Builder: create on a platform provider
- - Provisioner: configure the image post boot

### Configure Packer with Azure

- Required stuff:
- - Service principal
- - NIC
- - IP public
- - Subnet
- - Vnet
- `packer validate <file>`
- `packer build <file>`

## CI/CD

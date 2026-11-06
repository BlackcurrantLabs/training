# Infrastructure as Code (Terraform)

<img src="/assets/terraform.jpg" width="160">

## Topics

- Why "click-ops" doesn't scale
- Terraform basics: providers, resources, variables, outputs
- Workflow: `init`, `fmt`, `validate`, `plan`, `apply`, `destroy`
- State files - and why remote state matters even for practice projects
- Writing a reusable module

## How to learn

- [HashiCorp Terraform Tutorials](https://developer.hashicorp.com/terraform/tutorials) - official, free.
- [roadmap.sh/terraform](https://roadmap.sh/terraform) - a visual map of the full topic.

!!! note "Terraform vs OpenTofu"
    HashiCorp changed Terraform's license, so it's no longer fully open-source. [OpenTofu](https://opentofu.org/) is the open-source, drop-in-compatible fork - skills transfer 1:1 either way, and most job postings still say "Terraform," so learn that name first.

## How to practice

Recreate an AWS setup (EC2, S3, IAM, VPC) using Terraform instead of the console. Then destroy it and rebuild it with one command.

## Resources

- [HashiCorp Terraform Tutorials](https://developer.hashicorp.com/terraform/tutorials)
- [Terraform Documentation](https://developer.hashicorp.com/terraform/docs)
- [roadmap.sh/terraform](https://roadmap.sh/terraform)
- [OpenTofu](https://opentofu.org/)

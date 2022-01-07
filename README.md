## Consul-Terraform-Sync Test Module - Null

This Terraform module is used to test [Consul-Terraform-Sync](https://www.consul.io/docs/nia). It does not create any resources, which is helpful when trying to force the scenario of no infrastructure changes.

## Feature

This module uses the `null` Terraform provider and does not create any resources.

## Requirements

### Ecosystem Requirements

| Ecosystem | Version |
|-----------|---------|
| [consul](https://www.consul.io/downloads) | >= 1.7 |
| [consul-terraform-sync](https://www.consul.io/docs/nia) | >= 0.1.0 |
| [terraform](https://www.terraform.io) | >= 0.13 |

### Terraform Providers

| Name | Version |
|------|---------|
| local | >= 3.1.0 |

## Setup
There are no setup requirements for automating this module with Consul-Terraform-Sync.

## Usage

**User Config for Consul Terraform Sync**

example.hcl
```hcl
task {
  name           = "test"
  source         = "mkam/test/null"
  version        = "0.1.0"
  services       = ["web", "app"]
}
```

billing-account-iam
==================================================

# NAME

  billing-account-iam

# SYNOPSIS

  Config Connector compatible yaml files to enable permissions for a billing account.

# CONSUMPTION

  Using kpt:
  ```
  SRC=https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit.git
  kpt pkg get $SRC/config-connector/solutions/iam/kpt/billing-account-iam billing-account-iam
  ```

# USAGE
  Set the billing account, the IAM member to assign the role to, and,
optionally, the [billing
role](https://cloud.google.com/iam/docs/understanding-roles#billing-roles)
(defaults to viewer) to assign:
  ```
  kpt cfg set . billing-account VALUE
  kpt cfg set . iam-name VALUE
  kpt cfg set . billing-role admin
  ```

  Once your configuration is correct, apply it:
  ```
  kubectl apply -f .
  ```

# LICENSE
  Apache 2.0 - See [LICENSE](/LICENSE) for more information.

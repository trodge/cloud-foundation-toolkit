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

# SETTERS
|      NAME       |         VALUE          |     SET BY      |       DESCRIPTION        | COUNT |
|-----------------|------------------------|-----------------|--------------------------|-------|
| billing-account | ${BILLING_ACCOUNT_ID?} | PLACEHOLDER     | ID of billing account    | 1     |
| billing-role    | viewer                 | package-default | role to assign           | 1     |
| iam-name        | ${IAM_NAME?}           | PLACEHOLDER     | IAM member to grant role | 1     |
# USAGE

  Once your configuration is correct, apply it:
  ```
  kubectl apply -f .
  ```

# LICENSE
  Apache 2.0 - See [LICENSE](/LICENSE) for more information.

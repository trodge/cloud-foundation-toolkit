Secondary Ranges
==================================================
# NAME
  secondary-ranges
# SYNOPSIS
  Config Connector compatible YAML files for creating a simple VPC
# CONSUMPTION
  Download the package using [kpt](https://googlecontainertools.github.io/kpt/).
  ```
  kpt pkg get https://github.com/GoogleCloudPlatform/cloud-foundation-toolkit/config-connector/solutions/network/kpt/secondary-ranges secondary-ranges
  ```
# REQUIREMENTS
  A working Config Connector installation
# SETTERS
|     NAME     |          VALUE           |     SET BY      |   DESCRIPTION   | COUNT |
|--------------|--------------------------|-----------------|-----------------|-------|
| network-name | secondary-ranges-network | package-default | name of network | 5     |

# USAGE
  Configure using kpt as follows:
  ```
  kpt cfg set . NAME VALUE
  ```
  Setting placeholder values is required, changing package-defaults is optional.

  Once all values are satisfactory, apply:
  ```
  kubectl apply -f .
  ```
# LICENSE
  Apache 2.0 - See [LICENSE](/LICENSE) for more information.


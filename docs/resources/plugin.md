---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "sonarqube_plugin Resource - terraform-provider-sonarqube"
subcategory: ""
description: |-
  Provides a Sonarqube Plugin resource. This can be used to create and manage Sonarqube Plugins.
---

# sonarqube_plugin (Resource)

Provides a Sonarqube Plugin resource. This can be used to create and manage Sonarqube Plugins.

## Example Usage

```terraform
resource "sonarqube_plugin" "main" {
  key = "cloudformation"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `key` (String) The key identifying the plugin to uninstall.

### Read-Only

- `id` (String) The ID of this resource.
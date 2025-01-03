---
# generated by https://github.com/hashicorp/terraform-plugin-docs
page_title: "sonarqube_alm_gitlab Resource - terraform-provider-sonarqube"
subcategory: ""
description: |-
  Provides a Sonarqube GitLab Alm/Devops Platform Integration resource. This can be used to create and manage a Alm/Devops
  Platform Integration for GitLab.
---

# sonarqube_alm_gitlab (Resource)

Provides a Sonarqube GitLab Alm/Devops Platform Integration resource. This can be used to create and manage a Alm/Devops
Platform Integration for GitLab.

## Example Usage

```terraform
resource "sonarqube_alm_gitlab" "gitlab-alm" {
  key                   = "myalm"
  personal_access_token = "my_personal_access_token"
  url                   = "https://gitlab.com/api/v4"
}
```

<!-- schema generated by tfplugindocs -->
## Schema

### Required

- `key` (String) Unique key of the GitLab instance setting. Maximum length: 200
- `personal_access_token` (String, Sensitive) GitLab App personal access token with the `read_api` scope. See [this doc](https://docs.sonarqube.org/latest/devops-platform-integration/gitlab-integration/#importing-your-gitlab-projects-into-sonarqube) for more information. Maximum length: 2000
- `url` (String) GitLab API URL. Maximum length: 2000

### Read-Only

- `id` (String) The ID of this resource.
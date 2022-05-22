# tina

## About

Tina (Terraform inside Ansible) is a Ansible collection that works as wrapper around terraform execution.  
It brings the best of Ansible idempotence, templating and execution control to easily manage infrastructure as code.  



## Features

- Run/Extend terraform execution
- Idempotent changes on terraform state
- External secrets management (no secrets on state file)
- Can persist ansible data on state or workspace
- Git credentials for private modules
- Inverse target on root modules/resources
- State or resource parse/checks
- Create provider files if not exists
- Create remote backends if not exists
- Azure pipelines and Github actions integrations
- Kubernetes provision and deploy integrations


## TO-DO

- Modules
  - [ ] terraform_init   - Terraform init (private repos, backend config)
  - [ ] terraform_former - Terraform runner (plan, apply, destroy, output)
  - [ ] terraform_state  - Terraform state management  (move, import, remove)
  - [ ] terraform_save   - Ansible vars/facts to another state/workspace
  - [ ] pull_request     - Create/Update pull_request

- Filter plugins (state filtering)
  - [ ] stategrep (filter state by provider/resource/module)
  - [ ] state2inventory

- Lookup plugins 
  - [ ] tfstate
  - [ ] tfoutput
  - [ ] azdevops_pipeline
  - [ ] github_actions
  - [ ] azkeyvault

- Templating
  - [ ] Builtin mutable terraform data sources (yaml, json)
  - [ ] Extensible using custom infrastructure or application templates
  - [ ] Builtin infra roles
    - [ ] On-Prem Kubernetes (k3s, k8s)
    - [ ] Managed Azure Devops Project
    - [ ] Managed Github repository

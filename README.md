## Usage
Deploy an instance for doing general development work on.

Prior to executing playbook:
- Need to set proper user/group name in roles/baseconfig/vars/main.yml
- If using google compute engine, need the following environment variables:
  - GCE_CREDENTIALS_FILE
  - GCE_EMAIL
  - GCE_INI_PATH
  - GCE_PROJECT
- And a gce.ini in inventory. (clone from ansible repo)

```
ansible-playbook -i inventory/gce.py dev_up_gce.yml
```


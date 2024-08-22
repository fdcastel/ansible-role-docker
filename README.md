# ansible-role-docker

Ansible role for installing Docker Engine according to [official Docker instructions](https://docs.docker.com/engine/install/).

For Debian/Ubuntu only.



# Usage

## Install

On your project root, run:

```bash
# Creates requirements.yml
cat > requirements.yml <<EOF
- name: requires-docker
  src: https://github.com/fdcastel/ansible-role-docker
EOF

# Install it
ansible-galaxy install -r requirements.yml
```



## Example playbook

```yaml
- name: Requires Docker Engine on all hosts
  hosts: all
  roles:
    - role: requires-docker
```



## Uninstall

```bash
ansible-galaxy role remove requires-docker
```



## Requirements

None.



## Role variables

None.



## Dependencies

None.

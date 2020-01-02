# Portainer Agent

A role to add a Portainer Agent to the node as a Docker Service, including mounting the Docker socket and exposing port 9001. The role can be configured to specify a shared secret between agent and server, by setting an environment variable as follows: `PORTAINER_SECRET=sh33ghhw32rjhb3`.

## Usage

Include this role in a playbook using a [requirements.txt](https://galaxy.ansible.com/docs/using/installing.html#installing-multiple-roles-from-a-file) file.

### Example playbook

```yaml
- hosts: manager[0]
  roles:
    - portainer-agent
```

## Deployment

This role will be automatically built and deployed to [Ansible Galaxy](https://galaxy.ansible.com/gendall) when a [Semver](https://semver.org) tag is pushed to the repo.

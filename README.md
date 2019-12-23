# Portainer Agent

A role to add a Portainer Agent to the node as a Docker Service, including mounting the Docker socket and exposing port 9001. The role can be configured to specify a shared secret between agent and server, by setting an environment variable as follows: `PORTAINER_SECRET=sh33ghhw32rjhb3`.

## Example playbook

```yaml
- hosts: manager[0]
  roles:
    - portainer-agent
```

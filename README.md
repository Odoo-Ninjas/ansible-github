# ansible-github

Manages github repos access.


```yaml
github:
  hosts:
    localhost:
      connection: local
      repos:
        - repo: Odoo-Ninjas/my-project
          deploy-keys:
            - {{ inventory_dir }}/ssh_keys/fair.id_rsa
          webhooks:
            - http://host/trigger/repo/<project>/<password>

```

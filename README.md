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
            - url: http://host/trigger/repo/<project>/<password>
              events:
                - push

```

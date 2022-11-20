# ansible-github

Manages github repos access.


```yaml
github:
  hosts:
	localhost:
      connection: local
      ansible_user: "{{ lookup('env', 'USER') }}"
      configs:
        - repo:
			url: https://github.com/Odoo-Ninjas/fairever-dev
			deploy-keys:
			  - {{ inventory_dir }}/ssh_keys/fair.id_rsa

```

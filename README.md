# uWSGI Emperor

A role for installing and initializing uWSGI in emperor mode


## Requirements

This role requires that a specified version of Python is installed on the target host machines. See [Role Variables](#role-variables) for more information.


## Dependencies

- vforgione.python


## Role Variables

| name             | description                                                          | default | example |
| ---------------- | -------------------------------------------------------------------- | ------- | ------- |
| `python_version` | the version number of python to use for installing and running uWSGI | `3.5`   | `2.7`   |


## Example Playbook

```yaml
- hosts: django-apps
  become: yes
  become_user: root
  roles:
    - role: vforgione.uwsgi-emperor
      python_version: 3.5
```


## License

MIT


## Author Information

[Vince Forgione](https://github.com/vforgione)

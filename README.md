# Patch

Ansible role to embed patch module.

- Original `patch` module from
  [luisperlaz/ansible-misc-modules](https://github.com/luisperlaz/ansible-misc-modules)

- Reorganize filetree to fit `galaxy` and new repos to get a better galaxy name.

- Patch module to support `check-mode`

	SHA: ecee1b0d830917bc2f88998f1e47deaca293f799
	SHA: ecee1b0d

## Example Playbook

After declaring `patch` role:

```yaml
- hosts: all
  roles:
    - patch
```

You can use patch module:

```yaml
- name: Patch some paramiko code
  patch: patchfile=/tmp/critical.patch strip=1 basedir=/usr/share/pyshared/paramiko"
```

## Prerequisites:

GNU patch installed


## License

MIT

## Author Information

Thierry Delamare

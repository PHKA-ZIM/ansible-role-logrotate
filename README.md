# Logrotate automation with ansible

## Installation steps

- Go to you ansible project folder
- Add following to your requirements file

```
- src: https://github.com/PHKA-ZIM/ansible-role-logrotate
  name: ansible-role-logrotate
```

- Install to project roles path
```
ansible-galaxy install -r requirements.yml --roles-path ./roles
```

## Use ansible-role-logrotate

- Import role and override role variables, e.g.
```
- name: Setup logrotate
  roles:
    - role: ansible-role-logrotate
```

- All available role vars can be found in `defaults`

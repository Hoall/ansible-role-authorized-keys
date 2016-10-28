# Role authorized_keys

This role installs a list of ssh public keys in the authorized_ssh key file of the spezified user.

## Requirements

A ssh service.

## Role Variables

| Name                  | Default Value | Description                        |
| --------------------- | ------------- | -----------------------------------|
| `AUTHORIZED_KEYS_KEYLIST` | NONE | 'Define a list of public ssh keys.' |
|`authorized_keys_user_home` | '/root' | 'The user home directory to install the keys to.' |
|`authorized_keys_user` | 'root' | 'The user' |
|`authorized_keys_group` | 'root' | 'The group' |
|`authorized_keys_mode` | '600' | 'The authorized_keys file permissions.' |

## Dependencies

none

## Example Playbook

    - hosts: servers
      roles:
         - { role: hoall.authorized-keys }

## License

BSD

## Author Information

Felix Paetow fhmpaetow@fsfe.org


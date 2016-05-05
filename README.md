# Lasersaur

A simpe Ansible role to manage lasersaur app deployment

## Role Variables

```` yaml
lasersaur_repo: https://github.com/fablab-ka/LasaurApp
lasersaur_version: master

# backend/config.json
lasersaur_config:
  tolerance: 0.08
  serial_port: '/dev/ttyACM0'
  network_port: 80

lasersaur_user: lasersaur
lasersaur_daemon_name: lasersaur
lasersaur_dir: /opt/lasersaur
lasersaur_config_dir: /etc/lasersaur
lasersaur_allowed_ids_file: "{{ lasersaur_config_dir }}/idlist.txt"
lasersaur_admin_ids_file: "{{ lasersaur_config_dir }}/adminidlist.txt"

lasersaur_allowed_ids:
  - name: testkey1
    id: 71 4C 5C 88 6E 97
  - name: testkey2
    id: AA BB CC DD EE FF

lasersaur_admin_ids:
  - name: adminkey1
    id: 53 3C B6 C7 23 F6
````

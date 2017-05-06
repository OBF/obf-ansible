# obf-ansible - Ansible playbooks for OBF-run servers

Run in the following way:
```sh
$ ansible-playbook -i hosts <PLAYBOOK>
```

The following playbooks are currently available:
* `update-reboot.yml` - Runs `yum update -y` across the AWS-hosted inventory,
  and when complete reboots each one, waiting for each to come back.

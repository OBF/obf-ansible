# obf-ansible - Ansible playbooks for OBF-run servers

## Install dependencies

Playbooks here currently have the following dependencies:
* Ansible Galaxy roles:
    - `stafwag.package_update`
    - Install roles from Ansible Galaxy like this:
      ```sh
      $ ansible-galaxy role install <ROLE_NAME>
      ```
      They will install into the default directory, typically
      `~/.ansible/roles/` on Unix and macOS systems.

## Run the playbooks

Run in the following way:
```sh
$ ansible-playbook -i hosts <PLAYBOOK>
```

The following playbooks are currently available:
* `update-reboot.yml` - Runs OS-appropriate package updates across the
  AWS-hosted inventory, and when complete reboots each one, waiting for
  each to come back.

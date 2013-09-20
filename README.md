Ansible playbook to install standalone Red Hat Satellite Server v5. It will sync any products listed. It uses the ISO installation method.

## Usage ##
1. Clone this repo

        https://github.com/aweiteka/ansible-satellite5.git

2. Update inventory hosts file if not running locally
3. Update private_vars.yaml file and review vars in site.yaml
4. Run the playbook:

        ansible-playbook -i inventory site.yml

## Requires ##
 * RHEL 6
 * RHN subscription
 * A Satellite server ISO on target server
 * A Satellite certificate defining products to sync

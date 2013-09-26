Ansible playbook to install standalone Red Hat Satellite Server v5. It will sync any products listed. It uses the ISO installation method.

## Usage ##
1. Clone this repo

        https://github.com/aweiteka/ansible-rh-satellite5.git

2. Update inventory hosts file if not running locally
3. Copy custom_vars.template to custom_vars.yaml file and update. Also review vars in site.yaml

        cp custom_vars.template custom_vars.yaml

4. Run the playbook:

        ansible-playbook site.yaml -i inventory 

## Requires ##
 * RHEL 6
 * A subscription to RH Satellite Server v5. The system does not need to be registered and subscribed if RHN credentials are provided in `custom_vars.yaml`.
 * A Satellite server ISO image on remote server (http)
 * Your organization's Satellite certificate on remote server (http)

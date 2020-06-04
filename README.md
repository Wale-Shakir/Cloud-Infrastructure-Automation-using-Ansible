# Cloud-Infrastructure-Automation-using-Ansible
Automate virtual machines and services of public cloud platform using Ansible
In this project, the layout for code is a standard; each chapter has a playbook and a role. Playbook and roles are cloud-specific and to manage the cloud resources. Each chapter defines the whole cloud process, such as tasks/main.yml, which helps to execute the list of tasks. And vars/main.yml takes care of the variable defined in the tasks. vars/secrets.yml stores the login credential of the respective cloud.

Execution Command example:
ansible-playbook gce_playbook.yml -i roles/gce/inventory -e roles/gce/tasks/GCE_Task_main.yml -e roles/gce/vars/secret.yml -e roles/gce/vars/GCE_Vars_main.yml

Similarly, we can do for all other platforms.

#Setting up a Windows host usign Ansible

Create a file called vars.yml
```
---
ansible_user: yourusername
ansible_password: averystrongpassword
ansible_connection: winrm
ansible_winrm_transport: basic
ansible_winrm_server_cert_validation: ignore
ansible_port: 5986
```


Run with command
```
ansible-playbook iis.yml -i hosts 
```
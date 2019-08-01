# Install [MegaCLI](http://hwraid.le-vert.net/wiki/DebianPackages) on Debian 9 (stretch) with [Ansible](https://www.ansible.com/)

1. Clone this repository locally:
```git clone https://github.com/moovs/megacli.git```
2. Add your ssh-key to the host you want to install MegaCLI:
```ssh-copy-id -i ~/.ssh/id_rsa.pub user@host```
- This logs into the server host, and copies keys to the server, and configures them to grant access by adding them to the authorized_keys file.
3. Just set up your server's IP in hosts file for example:
``` 
[my_group]
my_domain ansible_ssh_host=192.168.0.0 ansible_ssh_user=my_user
```
4. And run: 
```ansible-playbook -i hosts ./roles/megacli/main.yml```
5. Simple way to get a status of RAID run next command:
```megacli -AdpAllInfo -aALL```
6. You have installed MegaCLI on your host :alien:


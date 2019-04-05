Install [MegaCLI](http://hwraid.le-vert.net/wiki/DebianPackages) on Debian 9 (stretch) with [Ansible](https://www.ansible.com/)

1. If you want to install MegaCLI for RAID status you need to make the first three steps the same as described above, just change it:<br />
```step 4```<br />
to:<br />
```ansible-playbook -i hosts ./roles/megacli/main.yml```
2. You have installed MegaCLI on your host :alien:

***
### Author
[Nikolay Ovsiannikov](https://www.linkedin.com/in/nikolay-ovsiannikov/) - LinkedIn

# Backup Cisco MDS using Ansible and NXOS, where My Mac has Python3, but Switches still have Python2 only
Environment: Cisco MDs 9710
Ansible 2.10 on Mac OS
Mac has Python3, Cisco has Python2


One of the crutial bits was specifying the remote (cisco) python interpreter in the hosts file.
[all:vars]
ansible_network_os=cisco.nxos.nxos
ansible_python_interpreter='/usr/bin/python'



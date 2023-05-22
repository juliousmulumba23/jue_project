
                                  ANSIBLE PLAYBOOK MODE


>>> Applied to all the servers in the hosts file

ansible-playbook -i hosts -e inventory=all playbookname.yml


>>> Applied to all the productions servers in the hosts file

ansible-playbook -i hosts -e inventory=prod-servers playbookname.yml


>>> Applied to all the 2 servers in the hosts file

ansible-playbook -i hosts -e inventory=server1:server2 playbookname.yml


>>> Applied to 1 server in the hosts file

ansible-playbook -i hosts -e inventory=server playbookname.yml

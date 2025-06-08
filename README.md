# Task2_Devops
⚙ How to Run

cd ~/ansible-ssh-task
ansible-playbook -i inventory.ini playbook.yml --ask-become-pass

What the Playbook Does

    Creates a user called devuser with a home directory and bash shell

    Adds devuser to the sudo group

    Creates the .ssh/authorized_keys file from a public key

    Disables password authentication in /etc/ssh/sshd_config

    Restarts the SSH service

    Creates /opt/devdir with 660 permissions owned by devuser

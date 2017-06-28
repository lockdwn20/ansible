**Setting Up the Playbook**

In order to utilize this playbook the following pre-requisites must be complete:

1. The remote system must already contain an administrator account for use by ansible that is not the root account
 
1. The user running ansible must have copied their ssh key to each server that they will be configuring:
	1. ssh-keygen
	1. ssh-copy-id REMOTE_USER@REMOTE_MACHINE

1. The ansible.cfg file must be placed into the ansible server /etc/ansible directory (this config ensures that logging is enabled

1. The /etc/ansible/hosts file needs to contain the appropriate hosts IP Addresses (hostname if DNS configured) to be configured


**Running the Playbook**

To run the playbook utilize the appropriate commands:

* ansible all -m ping -u REMOTE_USER  //this is to test connectivity

* ansible-playbook ansible_vm_cfg.yml -u REMOTE_USER -kK  //This will connect to the system as the user setup in the prerequisites, the kK options will ask for the user and sudo passwords. 


**ASSIGNMENT:**

Here is my COA with a suspense of 30 June for BLUE SYSTEMS TRACK personnel:

1. Watch: https://www.ansible.com/quick-start-video
1. Watch: https://www.ansible.com/webinars-training/introduction-to-ansible
1. Watch: GIT and Github Crash Course for Beginners https://youtu.be/SWYqp7iY_Tc
1. Using: http://docs.ansible.com/ansible/index.html

   Systems A and B will each organize internally with two groups (for a total of 4x). Each of these groups will develop an Ansible playbook to configure a Ubuntu or Centos host (group choice) as follows below. Do NOT include any .mil references in the code, comments, or commits.

Source-code for this Ansible playbook should be stored in a GIT repo. Each team-member should have at least one commit to this git repo. Private GIT hosting is available at bitbucket.com. We will RUN the script against a VM. If it works, you pass. The suspense is several weeks out so this doesn't interfere with current, scheduled training, but it will require both self-study, teamwork, and project-management, ie steady progress over time.

**Playbook Items**

Configure a VM with Ansible to:

1. configure static IPs

1. configure SSH to work with only certificates and not allow root logins

1. set DNS

1. set NTP server to tick.gatech.edu

1. create a user ${first_initial}${last_name}

1. add this user to sudoers

1. add an additional syslog file under /var/log/${username}-alerts so that all notice-level syslog is added to this file

1. log a NOTICE level syslog message to localhost each time the Ansible script is run.





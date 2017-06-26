ansible_vm_config: this is the ansible configuration file to be used to complete the assignment

Vagrantfile: this vagrant file can be used for initiating vagrant vms to test the ansible file**


**vagrant must be installed on your system for the Vagrantfile to work


ASSIGNMENT:
Here is my COA with a suspense of 30 June for BLUE SYSTEMS TRACK personnel:

1. Watch: https://www.ansible.com/quick-start-video
2. Watch: https://www.ansible.com/webinars-training/introduction-to-ansible
3. Watch: GIT and Github Crash Course for Beginners https://youtu.be/SWYqp7iY_Tc
4. Using: http://docs.ansible.com/ansible/index.html

   Systems A and B will each organize internally with two groups (for a total of 4x). Each of these groups will develop an Ansible playbook to configure a Ubuntu or Centos host (group choice) as follows below. Do NOT include any .mil references in the code, comments, or commits.

Configure a VM with Ansible to:
   - configure static IPs
   - configure SSH to work with only certificates and not allow root logins
   - set DNS
   - set NTP server to tick.gatech.edu
   - create a user ${first_initial}${last_name}
   - add this user to sudoers
   - add an additional syslog file under /var/log/${username}-alerts so that all notice-level syslog is added to this file
   - log a NOTICE level syslog message to localhost each time the Ansible script is run.

5. Source-code for this Ansible playbook should be stored in a GIT repo. Each team-member should have at least one commit to this git repo. Private GIT hosting is available at bitbucket.com. We will RUN the script against a VM. If it works, you pass. The suspense is several weeks out so this doesn't interfere with current, scheduled training, but it will require both self-study, teamwork, and project-management, ie steady progress over time.

Testing

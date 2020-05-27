# HW7CS312
Creates an Ansible controller that spins up 4 Alpine VM web servers

Instructions on setting up Hw 7:
Boot up pfsense, CentOS, and the four Alpine VMs. Let each VM initialize before starting the next VM
Sign into the CentOS vm as centosuser.

Run command ./HW7Ansible

If the included shell script fails to work, follow the subsequent steps to pull a fresh shell script:
Run command: sudo yum install -y git

Run command: git clone https://github.com/SJFoxs/HW7CS312.git

Run command: cd HW7CS312

Rerun command: ./HW7Ansible

The Script will go through all the necessary steps to complete the homework and pull/create the necessary files. There is still a need to go through the prompts that the Script will ask for.
The first prompt will ask for each ip of the Alpine VMs, please enter the ip address and press enter. It will prompt for each one individually, so don’t input more than one ip address at a time.

The second prompt will ask some specifications for the SSH key generation, please press enter three times.

The third prompt will ask if it is fine to send the SSH key to each Ansible vm, enter yes and the password for root.

The script will then run the playbook and return the contents of “index.html” from each web server.


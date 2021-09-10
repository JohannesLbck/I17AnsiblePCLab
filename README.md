# I17AnsiblePCLab
Small Repository, that uses Ansible for some basic configuration of Fedora PCs.
# How to use
sudo ansible-pull -U https://github.com/JohannesLbck/I17AnsiblePCLab.git
# Structure
local.yml contains pretasks and includes towards the actual tasks in /tasks
1. /tasks/packages.yml installs missing packages and removes unneeded ones
2. /tasks/filecopies.yml can be used to distribute files to all the PCs on which ansible pull was used, rn just a placeholder
3. /tasks/users.yml sets up a new user
4. /tasks/cronjobs.yml sets up a autoupdater, which checks the repository every 10 minutes, and reruns the playbook if changes are found

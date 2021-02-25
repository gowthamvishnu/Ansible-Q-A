# Ansible-Q-A
1)explain about ansible?
a)* ansible is an automation engine which automates software provisioning,configuration management and application deployment.which is an opensource configuration management         tool.
 * in detail: ansible is an automation engine or software which we can completely automate the software configuration management as well as  what ever the deployment we want to     do we can automate as well as provisioning the software on this machine what and all the softwares we should have and how should have completely using ansible.
 * ansible can contreol large no of servers and eases the administration and operations tasks.ansible can do simple configuration management and complex archestration.It has all     the features that config tools have plus it's very easy to learn and implement.


2)How ansible works?
a)If you trying to use ansible.we generally referes it as IAAC(infrastructure as a code)
  IAAC: if you have a machine and you want to define state of a machine,ypu will be defining everything using some kind of script or file which ansible try to read nd ansible        try to maintain the machine.
   or whatevaer you want to do or maintain the configuration of a machine you will be refferring it as in terms of a code.so we refer ansible as IAAC.
 
 3) why ansible?
 a)other tools in the market can be really complicated.
  * cost
  * huge overhead of infrastructure setup
  * complecated setup
  * pull mechanisum(need to install agent on you want to maintain)
  * lots of learning required.

4)properties of ansible?
* agentless
* relies on SSH
* uses python
* push mechanisum

5)what is an ansible configuraton file?what are the different locations and priority of ansible config file?
a)It is a configuration file for your ansible.we can do some setting in the ansible.cfg files like mention our inventory file location,host key checking ,etc...those setting are used by ansible while running the ansible playbooks or adhoc-commands.
defalut location of ansible.cfg is under root /etc/ansible/ansible.cfg which have the least priority while running playbooks.
we can define ansible configuration in  different loactions .the locations with priority from top to bottom
 ANSIBLE_CONFIG Environment varible
./ansible.cfg the current directory.
~/.ansible.cfg file present in home directory.
/etc/ansible/ansible.cfg default ansible.cfg file.
NOTE:Ansible will only use the configuration setting from the file which is found in this sequence first.it will not look for the settings in the higher sequence files if the setting not present in the file which is choosen for the deployment.ex:for example if we have a congfig file in the home directory but inventory file is not there in the config file  which is in the /home directory while executing playbook. it will not  look for the other configuration file locations. it just throws you an error.

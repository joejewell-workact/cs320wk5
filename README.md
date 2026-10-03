 # This project is for week 5 of cs320

The project consists of:
- an ansible playbook
- 3 html files (index, cats, dogs)
- this read me 
- a licence (to be added when configuring the repo)
- a gitignore

## Purpose
the purpose was to:
- practice installing and removing software
- copy files from the control to a managed host. 
- manage services
- rebooting a system and waiting for it to return 
- organize a project with gitignore
- Create a README and select an open source licence

## Required software
- python 
- ansible core 

## inventory config  
```

[lamp_servers]
lampserver ansible_host=10.2.37.50 ansible_user=joe

[lamp_servers:vars]
ansible_python_interpreter=/usr/bin/python3
```


## How to run
simply run this command after cloning repo (note: you will need to install ansible and make sure you have ssh access to the assets listed in inventory.)
```
ansible-playbook install.yml
```
```

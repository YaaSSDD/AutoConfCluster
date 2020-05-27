# Automatic configuraton with Ansible
##Set Global Variable !!!Feed_token gitlab!!! for example && add worker in:
``` 
emacs -nw /Auto-cluster/roles/Common/defaults/main.yml
``` 

##command

generate new roles model : 

``` 
 ansible-galaxy init PlayBookName
``` 


execute playbook : ansible-playbook -v --user root infrastructure.yml

execute with sudo passwd : ansible-playbook -v -K --user ghost infrastructure.yml 


##Command utile Docker


###check disk status
``` 
    df -a
    docker system df 
```
###free space docker

``` 
    docker image prune -a
    docker container prune
```
###after restart your roles for re-init Docker infra
# ansible_final
Ansible_final is a repo which allows to automatise configuration of servers. 

# Environment 
  
![alt text](https://github.com/zanekkk/pp5/blob/master/environment.png)

## Installation
Make sure you have installed ansible on your machine. 

1.
Clone repo: 

```bash
$ git clone https://github.com/zanekkk/automat.git
```

2.
Set every Ip for your servers in hosts.ini and playbook.yml


```python
[stats_server]#ip statistic server
12.123.123.123 ansible_user=ec2-user

[loadbalancers]#ip web server (frontend)
23.123.223.123 ansible_user=ec2-user

[app_nodes]#ip app server (backend)
52.29.187.81 ansible_user=ec2-user
52.59.217.26 ansible_user=ec2-user
```


## Usage

To install configuration on 

```bash
$ ansible-playbook -i hosts.ini playbook.yml 
```

## Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

Please make sure to update tests as appropriate.

## License
zanekkk

## Ansible Playbook - NGINX + TestInfra

Install the NGINX web server on Ubuntu, and perform tests using testinfra 
(https://testinfra.readthedocs.io/en/latest/)

Local execution for demo, in a productive environment it is necessary to make
adjustments and it is interesting run testinfra via CI

###### How to exec playbook & test
 
```bash
apt-get install -y python3-pip 
```

```
pip3 install pytest-testinfra
pip3 install ansible 
```
```
ansible-playbook playbook.yml 
```

```
py.test tests/infratest.py
```

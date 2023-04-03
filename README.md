# G2 Ansible IaC (Infrastructure as code) Wordpress

[Ansible doc](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)

## Roles
- [x] Essentials
- [x] Swap
- [x] Docker
- [x] Traefik
- [x] MySQL
- [x] Wordpress
- [x] Node exporter
- [x] Gitlab runner
- [x] Reboot

## Setup
```
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
```

## Run
Add ssh config host name to `hosts`
```
ansible-playbook setup.yml
```

## Vault
```
echo $(htpasswd -nB user) | sed -e s/\\$/\\$\\$/g
```

## Defaults
```
Swap: 2G
Traefik: auth
MySQL: auth
```

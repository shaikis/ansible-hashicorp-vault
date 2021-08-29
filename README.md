# hc-vault

```
HashiCorp Vault Installation using Ansible.

execute this module using below command. 

clone this reposity using "git clone https://github.com/shaikis/hc-vault.git"

create directory inventory " mkdir inventory"
create a file hosts inside the directory " touch inventory/hosts"
add entry "echo "[hashicorpvault]" >> inventory/hosts"
add second entry " echo "hashicorpvault.exmple.com" >> inventory/hosts"

Run the below command to install hashicorp vault: 
 
ansible-playbook -i inventory/hosts  hc-vault/tasks/main.yml

```

## To Check at server level:
```
export PATH=$PATH:/opt/vault/bin
echo "export PATH=$PATH:/opt/vault/bin" >> ~/.bashrc

export VAULT_ADDRESS=http://10.128.0.2:8200
echo "export VAULT_ADDR=http://10.128.0.2:8200" >> ~/.bashrc

```

## Initialize Vault:
```
vault operator init
```
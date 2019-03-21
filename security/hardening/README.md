## Hardening playbooks

##### It is recommended to run this playbook on test servers first in order to ensure it does not interrupt service on production servers. By using this repository you agree to not hold the owner of the repository liable for any damage that occurs by using these playbooks.



### How to use on local machine:


1. Install ansible:

```
brew install ansible
```


2. Download this repository and `cd` into the hardening directory:

```
git clone https://github.com/heywoodlh/macOS-playbooks
cd macOS-playbooks/security/hardening
```


3. Edit the variables in `inventory` file with desired configuration:

```
nano inventory
```


4. Once inventory is configured, run the playbook using the inventory file:

```
ansible-playbook -i inventory harden.yml
```


If you don't plan to use Ansible at all afterward, feel free to uninstall Ansible:

```
brew uninstall ansible
```


# ERP System

### Python Installation

Link related
https://www.vultr.com/docs/how-to-install-erpnext-open-source-erp-on-ubuntu-17-04-22771

- Before installing python, we need to install `software-properties-common` to avoid couldn't find package problem

```
sudo apt-get install software-properties-common
sudo add-apt-repository ppa:deadsnakes/ppa
```

- Then install python

```
sudo apt-get install python3.7 python3.7-dev python3.7-venv python3.7-doc python3-pip
```

- Now you have python on your VPS

### Install Ansible

- Ansible automates software provisioning, configuration management and application deployment.

```
sudo pip install ansible
```

## Installing MariaDB Server

- Add the MariaDB repository into the system.

```
sudo apt-key adv --recv-keys --keyserver hkp://keyserver.ubuntu.com:80 0xF1656F24C74CD1D8
sudo add-apt-repository 'deb [arch=amd64,i386,ppc64el] http://mirror.nodesdirect.com/mariadb/repo/10.3/ubuntu bionic main'
```

- Install MariaDB

```
sudo apt-get update
sudo apt -y install mariadb-server libmysqlclient-dev
```

- You will prompt to enter root password to MariaDB.
  <img src="./MariaDB_password_prompt" alt="MariaDB_password_prompt"/>

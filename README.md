# Onboarding Playbook Ubuntu

Configuração automática de máquinas ubuntu com Ansible

## 📍 Objetivo

Facilitar a inserção de novos desenvolvedores, instalando e configurando via ANSIBLE o que for necessário em sua workstation.

## 📍 Pré-requisitos 
Para o playbook funcionar com sucesso, o desenvolvedor deverá ter configurado em sua máquina:

- [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/intro_installation.html)
- Uma chave SSH

## 📍 Variáveis do projeto

**ansible_user** - o desenvolvedor deve inserir sua conta de usuário. Ex.: usuario

**ansible_private_key_file** - o caminho onde a chave ssh gerada pelo desenvolvedor foi salva. 
Ex.: ~/.ssh/chave_gerada.pub

**path_user** - caminho do usuário mac. Ex.: /Users/usuario

**user_name** - nome de usuário do git

**user_email** - email usado no git

## 📍 Rodando o playbook
```bash
$ git clone https://gitlab.globoi.com/devops-produtos-publishing/onboarding-playbook-ubuntu

$ cd onboarding-playbook-ubuntu

$ ansible-playbook -i hosts playbook.yml
```

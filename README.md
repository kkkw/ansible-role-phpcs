ANSIBLE-ROLE-PHPCS
=========

phpcsをインストールするロール  
ansible実行ユーザーのglobal領域にインストールする  
phpcsに下記オプションを設定する

-  encoding=utf8
-  colors=true
-  report_width=120

Requirements
------------

php5.3以上
composerが実行できること

Example
----------------    

## ansible.cfg

```
[defaults]
roles_path = ./roles
```

## requirements.yml

requirements.ymlをロールとして欲しいplaybook配下で実行する

 ```
   - src: https://github.com/kkkw/ansible-role-phpcs
     scm: git
     version: master
     name: phpcs
 ```
 ## インストールコマンド
  
 ```shell
$ ansible-galaxy install -r requirements.yml 
 ```
 
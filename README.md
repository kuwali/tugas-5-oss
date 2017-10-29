# Ansible Playbook untuk Phabricator dan OrangeScrum

Silahkan melihat lebih lanjut mengenai [Phabricator] dan [OrangeScrum].

Panduan instalasi [Ansible] ada di [sini].


## Deploying Phabricator

Jalankan perintah berikut untuk melakukan deployment.

```
$ ansible-playbook playbooks/deploy_phabricator.yml -i [host]
```

## Deploying OrangeScrum

Jalankan perintah berikut untuk melakukan deployment.

```
$ ansible-playbook playbooks/deploy_orangescrum.yml -i [host]
```

Apabila tidak dapat melakukan login, silahkan lakukan perintah berikut.
```
$ sudo mysql -uroot orangescrum -e "delete from os_session_logs;"
```
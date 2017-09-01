# Ansible Role Django

Ansible script to install and deploy django over Ubuntu server.

## Description

* Installs django and creates a project.  
* Optionally arguments include uwsgi setup, nginx(web server), database(mysql or postgresql) and nginx setup.


## Dependencies

- { role: ansible.role.update_ubuntu } 
- { role: micropyramid.mysql, mysql_server_password : 'password', when: database == 'mysql' } 
- { role: micropyramid.postgresql, when: database == 'postgresql' } 


## Example Playbook
-------------------------

Customize and run test.yml file 
eg: ansible-playbook -i host_file test.yml --roles-path=/your_directory

Note: Roles uwsgi_django_setup, nginx_django_setup are optional

## Packages

| Package | Description | Status | Apt | Yum | Homebrew |
| ------- | ----------- | ------ | --- | --- | -------- |
| [Vim](www.vim.org/) | Vim Editor | Required | OK | NaN | NaN |
| [Vim](www.vim.org/) | Vim Editor | Recommended | OK | NaN | NaN |


## License

MIT

Visit our Django web development page `Here`_

.. _Here: https://micropyramid.com/django-development-services/
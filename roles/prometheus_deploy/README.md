Prometheus Deploy
=========

This role installs Prometheus on your host, configure it and start the service

Role Variables
--------------

There is not much to be said here. The role has only one variable, that being: prometheus_release, which is used to get your desired release. By default it is set to linux os and amd64 arhitecture but you can change it however you want.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - prometheus_deploy

Author Information
------------------
    Creator: Alexandru Nișulescu
    Contact: alex.nisulescu1998@gmail.com
    Linkedin: https://www.linkedin.com/in/alex-nisulescu-45822b178/

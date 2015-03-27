Role Name
=========

A role that installs Redmine backlogs plugin

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

redmine_dir: /opt/redmine
RAILS_ENV: production
sudo_user: redmine

redmine_backlogs:
  story_trackers: "Bug,Story,Risk,Change,Incident"
  task_tracker: "Task"


Dependencies
------------

Redmine installed.


Example Playbook
----------------

    - hosts: servers
      roles:
         - redmine_backlogs

License
-------

BSD

Author Information
------------------

FORGE Service Lab, Pasi Kivikangas, pasi.kivikangas@digile.fi

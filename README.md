Role Name
=========

A role that installs Redmine backlogs plugin

Requirements
------------

Redmine


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

None


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

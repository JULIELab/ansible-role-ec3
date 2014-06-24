ansible-role-ec3
================

Ansible role to install EC3 functionality (CLUES + IM + LRMS plugins)

It includes playbooks to install:
- CLUES-0.89
- CLUES-CLOUD-0.90
- IM-0.4
- LRMS plugin from {CLUES-SLURM-0.1, CLUES-PBS-0.88, CLUES-SGE-0.88}

Usage
=====

In the "Front-end node",  depending on the LRMS that you want:
```yml
roles:
    - { role: 'amcaar.ec3', lrms: 'torque'}
    - { role: 'amcaar.ec3', lrms: 'sge'}
    - { role: 'amcaar.ec3', lrms: 'slurm'}
```

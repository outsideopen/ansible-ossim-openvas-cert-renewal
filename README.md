# Ansible Role: USM/OSSIM openvas certificate renewal

Updates the OpenVAS certificates on a USM/OSSIM appliance.

This is based on the instructions on this page [How do I resolve OpenVAS expired certificate issues?](https://success.alienvault.com/s/article/How-do-I-resolve-OpenVAS-expired-certificate-issues) 

## Requirements

An USM/OSSIM appliance

## Role Variables

| Variable                    | Default | Comments |
| :-------------------------- | :------ | :-----   |
| usm_openvas_cert_lifetime   | 1460    | Number of days the certificates should be made for |
| usm_openvas_cert_allowance  | 432000  | Number of seconds before expire a cert should be renewed | 

## Example Playbook

    - hosts: all
      roles:
        - outsideopen.ossim-openvas-cert-renewal

## License

MIT / BSD

## Author Information

This role was created in 2019 by [David Lundgren](https://www.github.com/dlundgren/).
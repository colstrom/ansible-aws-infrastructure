# ansible-aws-infrastructure

aws-infrastructure builds out things according to seemingly arbitrary conventions. They probably make sense, in the appropriate context.

[![Platforms](http://img.shields.io/badge/platforms-ubuntu-lightgrey.svg?style=flat)](#)

Tunables
--------
`O_o`

Dependencies
------------
* None

Example Playbook
----------------
    - hosts: servers
      roles:
         - role: telusdigital.aws-infrastructure
           required_systems:
             - application
             - database
           autodeploy_passthrough_enabled: yes
           using_load_balancers: yes
           elb_ssl_offload: yes
           elb_ssl_certificate_name: application.foo-production

License
-------
[MIT](https://tldrlegal.com/license/mit-license)

Contributors
------------
* [Chris Olstrom](https://colstrom.github.io/) | [e-mail](mailto:chris@olstrom.com) | [Twitter](https://twitter.com/ChrisOlstrom)
* Steven Harradine
* Justin Scott
* Aaron Pederson
* Ben Visser
* Kinnan Kwok
* Royston Tong

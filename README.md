# ansible-rhhi
Automated installation and management of [Red Hat Hyperconverged Infrastructure (RHHI)](https://www.redhat.com/en/technologies/storage/use-cases/hyperconverged-infrastructure) with Ansible.

## Overview
The Ansible Playbooks in this project are designed to be run via AWX in order to best manage Remote Office/Branch Office (ROBO) deployment scenarios of RHHI. An organization can have a centrally managed, distributed AWX deployment in their primary infrastructure, with AWX isolated instances deployed in each ROBO. These AWX isolated instances make it possible to properly orchestrate installation and management of many RHHI deployments, each in their own ROBO.

This project follows the [RHHI installation docs](https://access.redhat.com/documentation/en-us/red_hat_hyperconverged_infrastructure/1.0/html/deploying_red_hat_hyperconverged_infrastructure/). A few conventions are enforced in this project, like naming of RHHI hosts in inventory, so that the automation itself can be simpler. When first seeing this keep in mind that it does not affect the underlaying architecture of a RHHI deployment, just how that architecture is expressed in Ansible inventory.

## License
[GNU General Public License v3.0](LICENSE)

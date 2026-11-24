
## 1. Overview

This project aims to build an automated, cloud-based cybersecurity lab environment using Microsoft Azure. It is designed to simulate a small-scale enterprise infrastructure consisting of servers, clients, network components, identity management services, and security monitoring solutions.

The environment will provide a hands-on platform for experimenting with infrastructure management, endpoint monitoring, threat detection, security incident analysis, and cloud technologies.

## 2. Architecture

**Azure-based:**

- *Network* - VNet with DMZ subnets, LAN, and gateways. Everything protected by NSG rules
- *Servers* - Two Windows Server instances with Active Directory, DNS, and GPO
- *Endpoints* - Windows 10/11 and Linux clients
- *Gateway* - Secured for SIEM usage

**Other:**

- *Wazuh* - SIEM tool for collecting and analyzing security logs from whole lab environment
- *Zabbix* - Tool for monitoring the availability and performance of servers

## 3. Repository Structure

```text
├── Endpoints/
│   └── # Endpoint configurations and deployment files
│
├── Network/
│   └── # Network configurations and resources
│
├── SIEM/
│   └── # SIEM configuration, detection rules, logs and monitoring
│
├── docs/
│   └── # Project documentation
│
└── terraform/
    └── # Infrastructure as Code definitions
```

*More info about specific part of the project can be found in `README.md` in specific folder*

## 4. Setup

*Here will be requirements and step by step explanation of how to set up the project*

## 5. Documentation

#### General Info

Documentation is stored in the `docs` folder in the .md format. Every documentation and README file in this project is written in english.

Moreover, in the same location can be found `documentation_template.md` that shall be used as a guideline on how the documentation standard in this project is.
#### About New Documentation

Every project increment must be documented, be it in an existing documentation file or in a new one. It is advised to create a documentation after testing period but before completeing the task and/or closing an Issue. 

Every documentation must reflect the current state of the increment. Every test must be supported by evidence.

Creating and maintaining relevant documentation is a task that needs to be performed by the team responsible for the increment.

Documentation should follow the general project standard in the `documentation_template.md` with possible deviations when justified by specific project requirements. Every documentation file should be written in english.

After changing an existing documentation file remember to change the newest version and write who is the author of the most current version in the designated fields.

Never include passwords, access tokens, private keys, connection strings containing credentials, or other sensitive information.

## 6. Rules of Work

**Project**:

- *Sprints* - Every Sprint lasts for 2 weeks.
- *Issues* - Every task should be an Issue made on the original repository, and should be connected with the project's Kanban Board. Skipping this part won't be a crime I guess
- *Documentation* - Every team is held responsible for creating and updating documentation about increment made by them, and also for `README.md` in their specific folder.
- *Reporting* - Every team leader must report their achievments and possible blocks or errors on #raporty channel on discord
- *Tests* - Test should be made locally by team members via VirtualBox, Docker or their own Azure for Students account

**Repository:**

- *Forks* - To work on this project remember to create a fork or work on the fork created by the team leader
- *Pull Requests* - No changes should be committed directly to main branch. Use Pull Requests and Issues to Merge them with main in the original repository. Every PR needs to verified by at least one person, and should be notified on #raporty channel on discord

## 7. Disclaimer

This project is developed for educational and research purposes only.

All security testing, attack simulations, and experiments must be conducted within the designated lab environment or on systems for which explicit authorization has been granted.
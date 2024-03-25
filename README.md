# BugBounty-Toolbox

Welcome to BugBounty-Toolbox! This repository contains a collection of Ansible playbooks and roles designed to set up a versatile bug bounty hunting environment.

## Overview

BugBounty-Toolbox automates the setup and configuration of various tools and utilities commonly used in bug bounty hunting. It includes playbooks and roles for managing SSH configurations, installing utils, and opensource pentesting tools.
## Features

- Automates the setup of SSH configurations for secure access.
- Installs Golang and sets up environment variables.
- Performs reconnaissance tasks such as subdomain enumeration.

## Structure

The repository is structured as follows:

```
.
├── group_vars            # Group variables
│   └── all.yml           # Variables shared across all groups
├── inventories           # Inventory files
│   ├── main              # Main inventory
│       └── hosts         # Hosts file for the main inventory
├── playbook.yml          # Main Ansible playbook
├── README.md             # This README file
├── roles                 # Ansible roles directory
│   ├── golang            # Role for installing Golang
│   ├── recon             # Role for performing reconnaissance tasks
│   └── ssh               # Role for managing SSH configurations
└── testbook.yml          # Test playbook for development purposes
```

## Getting Started

To get started with BugBounty-Toolbox, follow these steps:

1. Clone this repository to your local machine.
2. Review the `group_vars/all.yml` file to customize variables as needed.
3. Execute the `playbook.yml` playbook using Ansible to configure your environment.

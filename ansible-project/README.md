# Ansible Sample Project

This repository contains a modular, clean sample Ansible project for web server configuration and artifact deployment.

## 📁 Directory Structure

```text
ansible-project/
├── ansible.cfg          # Ansible configuration file
├── inventory.ini        # Target host inventory
├── site.yml             # Main playbook
├── group_vars/
│   └── all.yml          # Global variables
└── roles/
    └── webserver/       # Webserver configuration role
        ├── tasks/
        │   └── main.yml # Tasks for webserver role
        ├── templates/
        │   └── index.html.j2 # HTML Jinja2 template
        └── vars/
            └── main.yml # Role-specific variables
```

## 🚀 How to Run

1. **Verify Playbook Syntax:**
   ```bash
   ansible-playbook -i inventory.ini site.yml --syntax-check
   ```

2. **Run in Dry-Run / Check Mode:**
   ```bash
   ansible-playbook -i inventory.ini site.yml --check
   ```

3. **Execute Playbook:**
   ```bash
   ansible-playbook -i inventory.ini site.yml
   ```

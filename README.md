![roboshop](https://github.com/user-attachments/assets/706a147d-6434-42bf-b576-987f68526079)

# Automation — Ansible Roles

This project refactors a traditional Ansible playbook–based deployment into a **role-driven automation system**, aligned with **DevOps and SRE best practices**.

The intent is simple: **make automation scalable, maintainable, and production-ready**.

## Why This Matters
- Uses DRY concept
- Roles enforce **separation of concerns**
- Faster debugging through **service isolation**
- Ready for CI/CD and GitOps workflows

## What Was Improved
- Migrated flat playbooks → **Ansible roles**
- One role per microservice (catalogue, user, cart, payment, shipping, frontend)
- Central orchestration via `main.yaml`
- Inventory-driven deployments

## How to Run
```bash
ansible-playbook -i inventory.ini main.yaml

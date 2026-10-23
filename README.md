# Copado_23102026

This repository has been initialized as an SFDX (Salesforce DX) project.

Project structure:

- `sfdx-project.json` – Salesforce DX project definition
- `config/project-scratch-def.json` – Scratch org definition
- `manifest/package.xml` – Deployment package manifest
- `force-app/` – Default source folder for Apex, Lightning, and static resources

Suggested folder layout:

```text
force-app/
  main/
    default/
      classes/
      triggers/
      aura/
      lwc/
      staticresources/
```

Common commands:

```bash
# Create a scratch org
sf org create scratch -f config/project-scratch-def.json -a CopadoScratch -d 30

# Push source to the scratch org
sf project deploy start -d force-app

# Open the scratch org
sf org open -o CopadoScratch
```

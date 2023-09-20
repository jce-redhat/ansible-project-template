[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)

# Ansible Project Template

A bare-bones repository template for Ansible projects which includes [ansible-lint](https://ansible.readthedocs.io/projects/lint/) and [pre-commit hook](https://pre-commit.com) configurations.  A [GitHub action for ansible-lint](https://github.com/marketplace/actions/run-ansible-lint) is also provided.

When the project uses Ansible content collections from [Red Hat Automation Hub](https://console.redhat.com/ansible/automation-hub), an [offline token](https://console.redhat.com/ansible/automation-hub/token) is required in order to download content.  For the ansible-lint GitHub action to work with content from Automation Hub, an [action secret](https://docs.github.com/en/actions/security-guides/using-secrets-in-github-actions) must be created wich contains the Automation Hub offline token.  The name of the secret must be "automation\_hub\_secret" (case insensitive) in order to match the action configuration.

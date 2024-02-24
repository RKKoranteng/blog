---
title: 'GitHub-Action: Resource Not Accessible By Integration'
author: Richard Koranteng
date: 2024-02-22 7:00:00 -0600
description: GitHub Action error that integration resource is not accessible 
categories: [Git,GitHub]
tags: [error,GitHub,Actions]
img_path: /assets/screenshots/2024-02-22-github-action-resource-not-assessiable
image:
  path: action-resource-integration-error.PNG
  width: 100%
  height: 100%
  alt: ansbible playbook for rds
---

## Issue
I ran into this issue when creating my first GitHub Actions release using `actions@create-release`{: .filepath}.

## Cause
When you delete a repository and recreate it with the same name, it is possible that some settings or permissions related to the integration (GitHub Actions) are not properly updated.


## Solution
Enable the workflow integration.

Go to the repository's settings, navigate to the "Actions" and select "General"
![Simple Ansible Playbook to Create RDS Instance](ansible-create-rds.png){: .shadow }{: .light }
![Simple Ansible Playbook to Create RDS Instance](ansible-create-rds.png){: .shadow }{: .dark }


Scroll down to the "Workflow permissions", select "Read and write permissions", then click "Save". This can help refresh the integration's access to the repository.
![Simple Ansible Playbook to Create RDS Instance](ansible-create-rds.png){: .shadow }{: .light }
![Simple Ansible Playbook to Create RDS Instance](ansible-create-rds.png){: .shadow }{: .dark }

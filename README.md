# project 12: ANSIBLE REFACTORING AND STATIC ASSIGNMENTS.

## Table of Contents.
- [Introduction](#introduction)
    - [Code Refactoring](#code-refactoring)
- [Prerequisites](#prerequisites)
- [Jenkins Job Enhancement](#jenkins-job-enhancement)


## Introduction
In this project, we would be refactoring the ansible code to make it more modular and reusable than the previous project. We would be learning how to create assignments, and learn how to use the imports functionality.

Imports allow us to effectively re-use previously created playbooks in a new playbook. This is a very powerful feature of Ansible and allows us to create a playbook that is very modular and reusable.

### Code Refactoring
Refactoring is a general term in computer programming. It means making changes to the source code without changing the expected behavior of the software. The main idea of refactoring is to enhance code readability, increase maintainability and extensibility, reduce complexity, and add proper comments without affecting the logic.

In this case, we would move things around a little bit in the code, but the overall state of the infrastructure would remain the same.


## Prerequisites
- Infrastructure: AWS.
- Web Servers: Linux Red Hat.
- Database Server: Ubuntu 20.04 + MySQL.
- Storage Server: Red Hat 8 + NFS.
- Load Balancer: Ubuntu 20.04 (Nginx).
- Jenkins Server.
- Configure Ansible.
- Source Code: Download from <a href="https://github.com/manny-uncharted/ansible-config-mgt.git">here</a>.


## Jenkins Job Enhancement
Before we begin, we need to make some changes to our Jenkins job, at the moment every new change in the codes creates a separate directory which is not very convenient when we want to run some commands from one place. Besides, it consumes space on the Jenkins server. So, we would be making some changes to the Jenkins job to make it more efficient.

- First, go to your Jenkins-Ansible server and create a new directory called 'ansible-config-artifact' we will store all artifacts after each build in the directory.

```
sudo mkdir /home/ubuntu/ansible-config-artifact
```

Results:

![make a directory to store build artifacts](img/)
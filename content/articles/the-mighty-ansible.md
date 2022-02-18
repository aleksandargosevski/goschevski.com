---
collection: posts
title: 'The Mighty Ansible'
description: 'I was always interested in automation tools, but they all seemed complicated. When a friend explained me in 5 minutes how Ansible works and how easy is to setup new project, I was amazed...'
createdAt: 2017-05-02
tags:
  - ansible
  - devops
---

I was always interested in automation tools, but they all seemed complicated. When a [friend](https://www.hcg.ninja/) explained me in 5 minutes how [Ansible](https://www.ansible.com/) works and how easy is to setup new project, I was amazed.

### What are the automation tools?

We use automation tools to automate machine or cluster of machines (infrastructure) setup. Imagine yourself SSHing to 100 servers and running same or similar commands to each one of them. Tools like Ansible could help you set up servers in parallel.

### How does Ansible works?

Ansible connects to your machines over SSH and runs tasks that you defined. After it finishes, it removes these tasks, so your machine stays clean and looks like you manually executed commands. It's using Python in the background, which most (if not all) systems have installed by default, so it does not require any pre-installation on the machines, and that's what makes Ansible so great.

Tasks that you write are text files (YAML), which means that you can store them on git. Because of this cool feature, you can have a history of changes you've made on your machines.

### How should I try it?

You can install Ansible on your machine and setup VMs using Vagrant. That's all you need to start. The good thing about this approach is that you can "develop" your infrastructure locally and then when you're ready, replace IPs of VMs to production machines inside config file.

### Tutorial

I'm pretty sure you can find a bunch of tutorials, so I won't write one, but I will share some useful links:

- [Ansible Docs](http://docs.ansible.com/ansible/intro.html)
- [Ansible Galaxy (tasks created by others)](https://galaxy.ansible.com)
- [Simple Ansible examples](https://github.com/ansible/ansible-examples)

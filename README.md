# ansible-nginx-webapp

Ansible Nginx Web App Deployment


## Description

This repository contains an awesome Ansible playbook for deploying a simple web application using Nginx as the web server. With Ansible, you can effortlessly set up and manage the entire deployment process, making it a breeze to get your web app up and running.


## Prerequisites
Before you proceed with the deployment, ensure you have the following:

- [x] A target server or VM with SSH access and a user with sudo privileges.
- [x] A registered domain name for your web app (required for Let's Encrypt SSL certificates).
- [x] An understanding of your web app's specific dependencies, if any.

## Getting Started

1. **Clone this repository:**

```bash
git clone https://gitlab.com/mka_devops-lab/devops/ansible-nginx-webapp.git
cd ansible-nginx-webapp

```

2. **Customize the playbook:**

- Edit the **hosts.yml** file and replace your-server-ip with the IP address or hostname of your target server(s).

- Modify group_vars/all.yml to suit your web app's installation requirements, including webapp name, web app port, ansible_user, and more.

3. **Run the the playbook to deploy the webapp:**

```bash
 ansible-playbook -i hosts.yml nginx_webapp_playbook.yaml
```

4. **Access to the web app:**

Once the playbook completes, access your web app by navigating to **https://your-domain.com** or **ip address** of the webserver in your web browser. 


## Troubleshooting

In case of any issues during the deployment, please refer to the Ansible documentation or open an issue in this repository.


## Author
[Mansour KA](http:mansourka.com)# ansible-webapp

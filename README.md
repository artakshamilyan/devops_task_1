# Stream Web Server Setup

This project provides an Ansible playbook and role to set up a web server on a Linux host that displays the latest frame from a given HTTP stream using NGINX and FFmpeg.

## Prerequisites

- Linux host
- Ansible installed
- Docker installed


### Installation

1. Clone or extract the repository containing the app files:
   ```bash
   git clone https://github.com/artakshamilyan/devops_task_1.git
   cd devops_task_1/ansible
2. Ensure necessary dependencies are installed:
	```bash
	sudo apt install ansible -y
	sudo apt install docker.io -y
	sudo systemctl start docker
	sudo systemctl enable docker
3. Run the following command to start the app:
	```bash
	ansible-playbook playbook.yml
4. Access the web server in your browser:
	```bash
	Access the web server in your browser:
### Notes
```
The NGINX container is set to run on port 8080.
Modify this in roles/stream_webserver/tasks/setup_nginx.yml if needed.

🧭 Project 1 — Linux Blog Hosting

Goal: Build a static blog from scratch, starting on your local Linux VM, then gradually move it to the cloud (AWS EC2), and finally automate deployment using DevOps practices.

✅ Phase 1 — Local Linux Environment (Core Linux Skills)

Objective: Understand and use Linux fundamentals to host a static website locally.

Checklist

 Install and configure a Linux VM (e.g., Ubuntu Server)

 Learn essential Linux commands (ls, cd, grep, chmod, systemctl, etc.)

 Set up user and file permissions correctly

 Install and start Nginx web server

 Create a simple index.html static page (blog homepage)

 Place files in /var/www/html and verify via localhost

 Configure basic firewall rules (ufw, iptables)

 Practice process management (ps, top, kill, systemctl restart nginx)

 Write your first bash script for a repetitive task (e.g., backup script or deploy script)

 Document all steps in a README.md

Outcome:
A static blog hosted locally on your Linux VM with full understanding of how it works.

☁️ Phase 2 — Cloud Hosting with AWS EC2 (Beginner Cloud Integration)

Objective: Replicate your local setup on a cloud Linux server.

Checklist

 Create an AWS Free Tier account

 Launch an EC2 instance using Ubuntu Server

 Configure Security Groups (open HTTP 80 + SSH 22)

 Connect via SSH

 Install Nginx + deploy your blog (same as on VM)

 Understand difference between local IP vs public IP

 Enable systemctl enable nginx for persistence

 Add a custom domain (optional) via Route 53 or any DNS provider

 Practice stopping/starting EC2, connecting, and managing uptime

Outcome:
You’ll see that EC2 is just a remote Linux machine — same commands, different location.

⚙️ Phase 3 — Automation & Industry Standard Practices

Objective: Deploy your project the way professionals do — automated, versioned, and secure.

Checklist

 Push codebase (HTML + config + scripts) to GitHub

 Write a clean README.md (setup, commands, architecture)

 Set up Git branching strategy (feature / main / test branches)

 Create a GitHub Action for CI/CD deployment to EC2

 Automate server setup using a bash script or Ansible playbook

 Configure a domain + SSL certificate (Let’s Encrypt)

 Add basic monitoring/logging (using journalctl, CloudWatch, etc.)

 Write a post-deployment checklist for debugging & maintenance

 Document your automation process in a DEPLOYMENT_GUIDE.md

Outcome:
Your static blog is hosted in the cloud, deployed automatically from GitHub, and maintained like a real DevOps project.

📘 Optional Stretch Goals

 Convert static HTML blog → Markdown + Static Site Generator (e.g., Jekyll / Hugo)

 Containerize with Docker + deploy via Docker Compose

 Use Terraform to create EC2 + Networking infrastructure

 Configure Nginx reverse proxy / load balancer

 Implement automated backups + monitoring scripts

🧾 Documentation Structure

Your repository could look like this:

project1-linux-blog/
│
├── README.md
├── PROJECT_GOALS.md        ← this file
├── DEPLOYMENT_GUIDE.md
├── scripts/
│   └── setup_server.sh
├── html/
│   └── index.html
└── .github/workflows/
    └── deploy.yml

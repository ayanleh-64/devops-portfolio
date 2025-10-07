
# 🌐 Linux Cloud Nginx Setup

## 🧠 Overview
This project sets up and configures an **Nginx web server** on an **Ubuntu VM**.  
It’s part of a broader DevOps learning roadmap to understand how Linux, web servers, and automation work together to host and manage web applications.

---

## ⚙️ Steps Taken

1. Updated system packages to get the latest software versions:
   
   ```sudo apt update && sudo apt upgrade -y```

2. Installed Nginx using apt:

   
   ```sudo apt install nginx -y```
3. Verified the Nginx service was running:

   
   ```sudo systemctl status nginx```
4. Tested connectivity using:

  ``` curl http://localhost```

5. Created a custom index.html and replaced the default Nginx page:

  ``` sudo cp index.html /var/www/html/index.html```


🏁 Outcome


Successfully hosted a custom static website inside the VM.

Gained hands-on experience with:

Linux package management

System services and process control

Basic HTTP server hosting

Replaced the default Nginx page with a custom static HTML blog.

🚀 Next Steps (Industry-Standard Improvements)

🔒 1. Secure the Server

Configure firewall rules with:

   
 ```   sudo ufw allow 'Nginx Full'
       sudo ufw enable```


Add HTTPS support using Let’s Encrypt via Certbot.

⚙️ 2. Automate Deployment

Create a simple Bash script (deploy.sh) to copy updated web files and reload Nginx:

   
```
#!/bin/bash
   echo "Deploying website..."
   sudo cp index.html /var/www/html/index.html
   sudo systemctl reload nginx
   echo "✅ Deployment complete!"```


Make it executable:


   ```
   chmod +x deploy.sh```


🧰 3. System Monitoring
Explore Nginx logs:


   ```
   sudo tail -f /var/log/nginx/access.log
   sudo tail -f /var/log/nginx/error.log```

Use journalctl -u nginx for service logs.


Learn about htop, df -h, and netstat for system monitoring.

☁️ 4. Cloud & DevOps Expansion
Host the VM on a cloud platform (AWS, Azure, or Google Cloud).

Integrate GitHub for version control and automated deployments (CI/CD).

Containerize Nginx with Docker for portability.

📘 Learning Goals
Deepen understanding of Linux administration.

Build foundations in DevOps, Automation, and Cloud Hosting.

Prepare for end-to-end pipeline integration with Bash and CI/CD tools.

👤 Author
Ayanleh Said
DevOps Learner | Linux Enthusiast | Exploring Cloud Automation

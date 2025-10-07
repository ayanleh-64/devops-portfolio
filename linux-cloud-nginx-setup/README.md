⚙️ Steps Taken

Updated package lists to ensure the latest software versions:

```
sudo apt update && sudo apt upgrade -y
```

Installed Nginx using apt:
```
sudo apt install nginx -y
```

Verified the Nginx service was running with systemctl:

```
sudo systemctl status nginx
```

Tested using curl to confirm that Nginx was serving pages:

```
curl http://localhost
```

Created a custom index.html and replaced the default page:

```
sudo cp index.html /var/www/html/index.html
```

🏁 Outcome

Successfully hosted a web server inside the VM.

Learned how to:

Install software packages with apt

Manage and verify system services

Test web server responses using curl

Replaced the default Nginx landing page with a custom static HTML blog.


🚀 Next Steps (Industry-Standard Improvements)

🔒 1. Secure the Server

Configure firewall rules with:

```
sudo ufw allow 'Nginx Full'
sudo ufw enable
```

Add HTTPS with Let’s Encrypt using Certbot.

⚙️ 2. Automate Deployment

Create a simple Bash script to deploy updates automatically:

```
#!/bin/bash
echo "Deploying website..."
sudo cp index.html /var/www/html/index.html
sudo systemctl reload nginx
echo "✅ Deployment complete!"
```

Make it executable:

```
chmod +x deploy.sh
```
🧰 3. Explore Logs & Monitoring

View Nginx access logs:

```
sudo tail -f /var/log/nginx/access.log
```

View Nginx error logs:

```
sudo tail -f /var/log/nginx/error.log
```

Check service logs with:

```
journalctl -u nginx
```

☁️ 4. Cloud & DevOps Expansion

Host the VM on a cloud provider (AWS, Azure, or Google Cloud).

Integrate GitHub for version control and CI/CD automation.

Containerize the Nginx setup using Docker for portability and scalability.

📘 Learning Goals

Strengthen Linux administration fundamentals.

Gain hands-on experience with server configuration and deployment.

Build toward full DevOps automation with Bash and CI/CD pipelines.

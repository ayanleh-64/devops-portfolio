# Linux Cloud Nginx Setup

## Overview
This project sets up an Nginx web server on an Ubuntu VM. 
The goal is to practice Linux package management, system services, and server configuration. 

## Steps Taken
1. Updated package lists to ensure latest software versions.
2. Installed Nginx using `apt`.
3. Verified the Nginx service was running with `systemctl`.
4. Testing with curl: I used `curl` to confirm that Nginx was serving pages:

## Outcome
- Successfully hosted a web server inside the VM.
- Learned how to install software, manage services, and test web traffic.

## Next Steps (Industry Standard Improvements)
- Replace default page with custom static HTML blog. 
- Configure firewall rules with `ufw`.
- Add HTTPS with Let's Encrypt (Certbot).
- Automate setup with a Bash script. 
- Explore Nginx logs and monitoring (`journalctl`, `/var/log/nginx/`)

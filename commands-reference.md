# Commands Reference

## EC2 Setup
- `sudo apt update && sudo apt upgrade -y`
- `sudo apt install nginx -y`
- `sudo systemctl start nginx && sudo systemctl enable nginx`

## Domain Setup
- Route 53 A Record → EC2 public IP
- CNAME Record → root domain

## SSL
- `sudo apt install certbot python3-certbot-nginx -y`
- `sudo certbot --nginx`
- `sudo certbot renew --dry-run`

# Commands Used

## Connect to EC2

```bash
ssh -i aws-web-server-key.pem ubuntu@<PUBLIC-IP>
```

## Update Packages

```bash
sudo apt update
sudo apt upgrade -y
```

## Install Apache

```bash
sudo apt install apache2 -y
```

## Check Apache Status

```bash
sudo systemctl status apache2
```

## Enable Apache

```bash
sudo systemctl enable apache2
```

## Restart Apache

```bash
sudo systemctl restart apache2
```

## Verify Port 80

```bash
sudo ss -tulnp | grep :80
```

## Upload Website Files

```bash
scp -i aws-web-server-key.pem index.html style.css script.js ubuntu@<PUBLIC-IP>:/home/ubuntu/
```

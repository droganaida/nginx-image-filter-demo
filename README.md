## How to install Image Filter module on Ubuntu

### 1. Add repository
```bash
sudo add-apt-repository "deb http://nginx.org/packages/ubuntu/ $(lsb_release -s -c) nginx"
```

**OR**
**Add the following line to /etc/apt/sources.list:**
eoan - your Ubuntu version (Codename)
```
deb http://nginx.org/packages/ubuntu/ eoan nginx
```

Check Ubuntu version
```
lsb_release -a
```

Open file:
```
sudo nano /etc/apt/sources.list

### 2. Install GPG key of the repository:
```
wget https://nginx.org/keys/nginx_signing.key && sudo apt-key add nginx_signing.key
```

### 3. Update the package index:
```
sudo apt-get update
```

### 4. Install nginx-module-image-filter deb package:
```
sudo apt-get install nginx-module-image-filter
```

## Popular Nginx Commands

**Start NGINX**
```
sudo systemctl start nginx
```

or 
```
sudo service nginx start 
```

**View Server Status**
```
systemctl status nginx
```

or 
```
sudo service nginx status
```

**Restart NGINX**
```
sudo systemctl restart nginx
```

or
```
sudo service nginx restart
```

**Reload NGINX**
```
sudo systemctl reload nginx
```

or
```
sudo service nginx reload
```

**Test Nginx Configuration**
```
nginx -t
```

**Stop NGINX**
```
sudo systemctl stop nginx
```

or
```
sudo service nginx stop
```

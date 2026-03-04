# Avon Talking Magazine Website
Repository for ATM Website

## Deployment Instructions

### GitHub Pages Setup
This site is configured to be hosted on GitHub Pages at: **avontm.co.uk**

### DNS Configuration Required
To connect your custom domain `avontm.co.uk`, configure these DNS records at your domain registrar:

**For apex domain (avontm.co.uk):**
```
Type: A
Host: @
Value: 185.199.108.153
```
```
Type: A
Host: @
Value: 185.199.109.153
```
```
Type: A
Host: @
Value: 185.199.110.153
```
```
Type: A
Host: @
Value: 185.199.111.153
```

**For www subdomain:**
```
Type: CNAME
Host: www
Value: jramsbottom.github.io
```

### Steps to Deploy:
1. Push this repository to GitHub
2. Go to repository Settings → Pages
3. Set Source to "Deploy from a branch"
4. Select branch: `main` and folder: `/ (root)`
5. Wait for GitHub to recognize the CNAME file
6. Update DNS records at your domain registrar (remove Wix DNS records)
7. Wait for DNS propagation (can take up to 48 hours, usually much faster)
8. Enable "Enforce HTTPS" in GitHub Pages settings once DNS is active

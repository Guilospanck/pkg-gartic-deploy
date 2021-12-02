# PKG Gartic Deploy

## Clone

```bash
git clone --recurse-submodules https://github.com/Guilospanck/pkg-gartic-deploy.git

git submodule update --init --recursive
```
### OBS.: verify if all repositories are really updated (git pull on them)

## Get Started

### Development
```bash
docker-compose -f docker-compose-development.yml up -d --build
```

### Staging
```bash
// docker-compose -f docker-compose-staging.yml up -d  --build
```

### Production
```bash
// docker-compose -f docker-compose-production.yml up -d --build
```

### Current Staging Server
---
- **Public IP:** <public-ip>
- **Public DNS:** ec2-<public-dns>.compute-1.amazonaws.com
---
- **Proteu**              - <public-ip>:3000
---
- **Gerdau**              - <public-ip>:3333
---
- **API**                 - <public-ip>:4444
---
- **IoT Websocket**       - <public-ip>:5555
---
- **PostgreSQL**          - <public-ip>:7568
  - User: pg_user
  - Password: 
---
- **Portainer**           - <public-ip>:9000
  - User: portainer_user
  - Password: 
---
- **Jenkins**           - <public-ip>:8080
  - User: jenkins_user
  - Password: 
---

### Add other projects

```bash
git submodule add -b develop https://REPOSITORY.git 
```
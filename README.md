# PKG Gartic Deploy
Simple application created using ReactJS with TypeScript for the frontend and Go for the backend. It makes use of Clean Code Architecture, Domain Driven Design and some Design Patterns.

## Frontend
- ReactJS with TypeScript
- Redux and Redux-Saga
- Styled-Components
- Jest
- Domain Driven Design

## Backend
- REST API in Go
- Go Gorilla WebSockets
- GORM
- Clean Code

## Database
- PostgreSQL

## Application
- ✅ Choose your name
- ✅ Choose your room or create a new one

<div align="center">
<img align="center" alt="part1" src="https://user-images.githubusercontent.com/22435398/144692015-873f8782-8039-4ef0-9f22-fa378e19f434.gif" style="max-width: 100%;">
</div>
<br>

- ✅ Multiple colors to draw
- ✅ Know which player is currently drawing
- ✅ Know which participants are in the room
- ✅ Progress Bar shows you how much time you have to draw or to get it right

<div align="center">
<img align="center" alt="part2" src="https://user-images.githubusercontent.com/22435398/144692178-5b3f711d-84b5-4e86-a60b-b129d1724395.gif" style="max-width: 100%;">
</div>
<br>

- ✅ Clear and erase functions
- ✅ Chat between participants

<div align="center">
<img align="center" alt="part3" src="https://user-images.githubusercontent.com/22435398/144692253-8b759e6e-6441-4b1c-8c21-5f0d2e214774.gif" style="max-width: 100%;">
</div>
<br>

- ✅ Multiple clients
- ✅ Multiple rooms

<div align="center">
<img align="center" alt="part4" src="https://user-images.githubusercontent.com/22435398/144692340-570641ac-8ac5-4bd4-ac58-eb1fb99a08cc.gif" style="max-width: 100%;">
</div>

## Clone

```bash
git clone --recurse-submodules https://github.com/Guilospanck/pkg-gartic-deploy.git

git submodule update --init --recursive
```
👉 OBS.: verify if all repositories are really updated (git pull on them)

## Get Started

### Development
```bash
docker-compose -f docker-compose-development.yml up -d --build
```

### Staging
```bash
docker-compose -f docker-compose-staging.yml up -d  --build
```

### Production
```bash
docker-compose -f docker-compose-production.yml up -d --build
```

### Current Staging Server
---
- **Public IP:** ```<public-ip>```
- **Public DNS:** ec2-```<public-dns>```.compute-1.amazonaws.com
---
- **Gartic**                    - ```<public-ip>```:3333
---
- **Go API**                    - ```<public-ip>```:8000
---
- **Go Websocket**              - ```<public-ip>```:5555
---
- **PostgreSQL**                - ```<public-ip>```:7568
---

### Add other projects
```bash
git submodule add -b develop https://REPOSITORY.git 
```

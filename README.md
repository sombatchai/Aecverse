# AECverse: Biogas Digital Twin Safety Training

A multiplayer 3D web platform where trainees practise biogas-plant safety together. Everyone enters a shared 3D space, uploads and adjusts models of the plant, and sees each other's changes in real time.

Built for **Accepted Engineering & Consultant Co., Ltd.** by a 3-person university team.

**Live demo:** https://aecverse.up.railway.app

![Digital twin](https://chatthadasainoi-cmyk.github.io/portfolio/img/aec-twin.jpg)

## Why it exists
- **Engineers can't be on every site.** AE&C's engineers travel between plants, and buyers often can't visit. Anyone can now walk the plant online, from anywhere.
- **New staff have never seen the real plant.** A mistake on real equipment is costly and dangerous. Workers learn how each unit works, take quizzes and try it hands-on in the digital twin first, including a VR mode on Meta Quest 2.
- **One place to explain the system** to contractors and workers, instead of repeated site visits.

| 26 | 32 | 20+ |
|---|---|---|
| web pages | API endpoints | real-time socket events |

## Features
- Shared 3D world with avatars and real-time model sync (Socket.IO)
- Upload, place and adjust 3D models of the plant; admin lock/unlock
- Plant zones with safety rules, risks, PPE and simulated IoT readings
- Hazard view: methane spread (LEL) and hazard radius
- Emergency flow: an alert moves everyone in the 3D world to the assembly point
- Sign-in with Google OAuth or Email OTP (Supabase Auth)

## Tech stack
JavaScript · Three.js · Node.js · Express · Socket.IO · Supabase · Vercel (client) · Railway (server)

## My role
**Scrum Master & backend lead.** Ran the sprints with the client; built the Node.js/Express server, Socket.IO real-time sync and Supabase storage; re-architected the codebase to remove layered patches; fixed cross-browser model sync by keying meshes on stable names instead of per-session IDs; added Google OAuth / Email OTP; deployed on Vercel and Railway.

## Run locally
```bash
npm install
npm start          # http://localhost:3000
```
Admin user management needs `SUPABASE_SERVICE_ROLE_KEY` set as an environment variable.

## Screens
![Sign-in](https://chatthadasainoi-cmyk.github.io/portfolio/img/aec-login.jpg)
![Virtual tour](https://chatthadasainoi-cmyk.github.io/portfolio/img/aec-tour.jpg)
![Hazard view](https://chatthadasainoi-cmyk.github.io/portfolio/img/aec-hazard.jpg)

---
Portfolio: https://chatthadasainoi-cmyk.github.io/portfolio/


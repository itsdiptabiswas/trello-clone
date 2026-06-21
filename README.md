A full-featured kanban-style project management board with live collaboration, built with React, TypeScript, and Socket.io. Create boards, organize work into lists, and move cards around — with every change syncing instantly across all connected users.
 
🔗 **[Live Demo](https://trello-clone-76971.web.app/)** &nbsp;·&nbsp; **[GitHub](https://github.com/itsdiptabiswas/trello-clone)**
 
---
 
## Features
 
- **Real-time collaboration** — board updates sync instantly to all connected users via Socket.io — no refresh needed
- **Boards, lists & cards** — full CRUD for boards, nested lists, and draggable cards
- **Drag and drop** — reorder cards and move them across lists with smooth interactions
- **Image attachments** — upload and attach images to cards via Cloudinary
- **User authentication** — secure login and session handling
- **Responsive layout** — works cleanly across desktop and mobile
- **Automated CI/CD** — GitHub Actions builds and deploys on every push to main
---
 
## Tech Stack
 
| Layer | Technology |
|---|---|
| Framework | React 18, TypeScript |
| State | Redux Toolkit, Redux Saga |
| Real-time | Socket.io |
| Styling | Bootstrap, SCSS |
| Media | Cloudinary |
| CI/CD | GitHub Actions |
| Hosting | Firebase |
 
---
 
## Getting Started
 
```bash
# 1. Clone the repo
git clone https://github.com/itsdiptabiswas/trello-clone.git
cd trello-clone
 
# 2. Install dependencies
npm install
 
# 3. Start the dev server
npm start
# → http://localhost:3000
```
 
### Production Build
 
```bash
npm run build
# Outputs to /build — minified, hashed, ready to deploy
```
 
---
 
## How It Works
 
**State management with Redux Saga**
All async operations — API calls, socket event listeners, optimistic updates — run through Redux Saga. This keeps reducers pure and makes the data flow easy to trace and test.
 
**Real-time sync with Socket.io**
When a user moves a card or updates a board, the change is emitted via Socket.io and broadcast to all active sessions. The UI updates immediately without a round-trip page reload.
 
**CI/CD with GitHub Actions**
Every push to `main` triggers the pipeline — install, build, and deploy to Firebase. No manual deployment steps.
 
---
 
## Screenshots
 
![Board overview](https://user-images.githubusercontent.com/46165735/185036506-1db7d6ab-b58f-4354-aff4-85e459a77b71.png)
 
![List and card view](https://user-images.githubusercontent.com/46165735/185036554-900cb389-37af-4d93-b523-91146d173730.png)
 
![Card detail](https://user-images.githubusercontent.com/46165735/185036577-345e9077-399b-4f04-9677-08116e73d4a5.png)
 
![Drag and drop](https://user-images.githubusercontent.com/46165735/185036622-ef7d76ef-fdb8-41db-aa67-d51e751a889a.png)
 
![Create board](https://user-images.githubusercontent.com/46165735/185036670-f65a2f43-62a2-495a-80fc-482a8d783b21.png)
 
![Mobile view](https://user-images.githubusercontent.com/46165735/185036748-2ae2505b-b02a-4fbe-bcd1-fa1f721d1c16.png)
 
![Auth screen](https://user-images.githubusercontent.com/46165735/185036790-2535de6a-e311-47f4-81c2-f60433cba073.png)
 
![Card attachments](https://user-images.githubusercontent.com/46165735/185036885-6acd0fb2-55a2-4c08-a3d7-ed9bd7238896.png)
 
![Real-time update](https://user-images.githubusercontent.com/46165735/185036926-b36f3122-d930-48f7-bb19-a333bc4e0472.png)
 
---
 
## Roadmap
 
- [ ] File and document attachments on cards
- [ ] Board background image customization
- [ ] Rich text / markdown in card descriptions
- [ ] Advanced commenting with mentions and reactions
- [ ] Card due dates with calendar view
---
 
## Author
 
**Dipta Biswas** — Senior Frontend Engineer specializing in React, TypeScript & real-time UIs
 
[LinkedIn](https://www.linkedin.com/in/dipta-biswas) · [GitHub](https://github.com/itsdiptabiswas) · [MBOX Project](https://drive-clone-ecru.vercel.app)

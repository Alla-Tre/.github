# AllaTre

**AllaTre** is a real-time online auction platform built to support structured, transparent, and competitive C2C auctions, with a strong focus on the Egyptian market.

<p align="center">
  <img src="https://img.shields.io/badge/status-active-brightgreen" />
  <img src="https://img.shields.io/badge/backend-Node.js%20%7C%20FastAPI-blue" />
  <img src="https://img.shields.io/badge/frontend-React%20Native%20%7C%20React-61DAFB" />
  <img src="https://img.shields.io/badge/database-PostgreSQL-336791" />
  <img src="https://img.shields.io/badge/license-MIT-lightgrey" />
</p>

---

## 📖 Overview

AllaTre enables users to create and participate in timed auctions with live bidding, reserve prices, and instant updates. The platform solves the limitations of traditional classified marketplaces by providing a complete auction lifecycle with real-time interaction — from listing creation to bidding, counter-offer negotiation, and final settlement.

---

## 🎥 Demo

### 📱 Mobile App Demo

<!-- Replace the link below with your GitHub user-attachments video URL -->
https://www.youtube.com/watch?v=Q6anT52n7e8
### 🖥️ Admin Dashboard Demo

<!-- Replace the link below with your GitHub user-attachments video URL -->
https://drive.google.com/file/d/1x4QfupKQx8ilbjKITBsxrwpKZq4jaUg5/view?usp=sharing

> **How to add your videos:** drag and drop the `.mp4` file into any GitHub issue/PR comment box, wait for it to upload, then copy the generated `https://github.com/user-attachments/assets/...` link it inserts and paste it in place of the placeholders above. GitHub will render it as an inline playable video.

---

## ✨ Key Features

- Timed auctions with automatic state management
- Real-time bidding using WebSockets
- Reserve price & Buy It Now support
- Secure bid validation and winner determination
- Post-auction counter-offer negotiation
- Ratings, reviews, reporting, and admin moderation
- Real-time notifications (outbid, auction ending, auction won)

## 🤖 AI Features

- **Semantic Search** — hybrid keyword + vector search for accurate auction discovery
- **Recommendation System** — personalized, context-aware suggestions based on user interactions
- **Policy-aware Chatbot (RAG)** — retrieval-augmented assistant for legal/policy questions

---

## 🏗️ Architecture

<p align="center">
  <img src="./ArchDiagram.png" alt="AllaTre System Architecture" width="800"/>
</p>

- Modular monolithic core backend (Node.js/Express)
- Separate FastAPI AI service (search, recommendations, RAG chatbot)
- Shared PostgreSQL (+ pgvector) data layer
- Secure REST APIs and WebSocket (Socket.IO) real-time channels

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| **Core Backend** | Node.js, Express |
| **AI Backend** | FastAPI (Python) |
| **Mobile App** | React Native (Expo) |
| **Admin Dashboard** | React.js / Next.js |
| **Database** | PostgreSQL, pgvector |
| **Cache** | Redis (Upstash) |
| **Real-time** | WebSockets (Socket.IO) |
| **Search & AI** | Meilisearch, FAISS, embedding models |
| **Media / Auth / Notifications** | Cloudinary, Akedly (OTP), Google OAuth, Expo Push |

---

## 📦 Repositories

| Component | Description | Repo |
|---|---|---|
| Core Backend | Node.js/Express transactional API | [`allatre-backend`](#) |
| AI Backend | FastAPI search, recs & chatbot service | [`allatre-ai-service`](#) |
| Mobile App | Expo / React Native client | [`allatre-mobile`](#) |
| Admin Dashboard | Next.js moderation console | [`allatre-admin`](#) |

> Update the links above to point to your actual GitHub repos.

---

## 🚀 Getting Started

Each service has its own setup instructions in its repository README. General flow:

```bash
# Clone the repo you need
git clone <repo-url>
cd <repo-folder>
npm install   # or pip install -r requirements.txt for the AI service
```

Refer to each repository's `.env.example` for required environment variables.

---

## 🧪 Testing

All four services include automated test suites (Jest for Node.js/mobile/admin, pytest for the AI service). See each repo for coverage details and how to run tests locally.

---

## 📄 License

This project is licensed under the MIT License — see the `LICENSE` file for details.

---

**AllaTre — Fair, real-time online auctions.**

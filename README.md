# 🚀 Challenge 20: Testing

## Overview

This project demonstrates a fully operational CI/CD pipeline using **GitHub Actions**, **Cypress**, and **Render**. It showcases a professional workflow that runs component tests on every pull request and automatically deploys the application when updates are merged into the `main` branch.

## Key Features

- ✅ **Cypress Component Tests** run on PRs to `develop`
- ✅ **Deployment to Render** when `main` is updated
- ✅ Written in **TypeScript** using Node.js + Express backend
- ✅ React frontend scaffolded with Vite
- ✅ GitHub Actions automation using two separate workflows

---

## Live Application

**Git and Render Links:**  
[https://challenge-20-api.onrender.com]https://github.com/shawnachirillo/challenge-20.git


---

## CI/CD Workflow

### Cypress Workflow
- Triggered when a **pull request is made to `develop`**
- Runs `npx cypress run --component`
- Fails the PR if tests do not pass

### Deploy Workflow
- Triggered when changes are **pushed or merged to `main`**
- Calls a **Render Deploy Hook URL** via `curl`
- Ensures the production app stays up-to-date automatically

---

## Tech Stack

- React
- Vite
- TypeScript
- Node.js
- Express
- MongoDB
- Cypress
- GitHub Actions
- Render

---

## How to Run Tests Locally

```bash
npm install
npx cypress open

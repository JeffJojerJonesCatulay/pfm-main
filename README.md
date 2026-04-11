# Personal Finance Manager

The **Personal Finance Manager** is designed to help users track, allocate, and manage their finances in one intuitive interface. It provides a friendly dashboard with quick access to essential financial tools, making financial management simple and effective.

✅ **Project Status:** Completed on **April 11, 2026**, but not limited for future enhancements, added features, and bug fixes.

## Features

- 📊 **Dashboard Overview**  
  Get a clear snapshot of your financial health with income, expenses, and savings displayed in one place.

- 💰 **Expense Tracking**  
  Record and categorize your daily spending to identify patterns and areas for improvement.

- 🗂️ **Budget Allocation**  
  Set budgets for different categories and monitor progress to stay on track.

- 📈 **Financial Insights**  
  Visualize trends with charts and reports to make informed decisions.

## 🚀 Project Showcase

Experience the full visual tour and documentation portal for the PFM ecosystem:
👉 **[Personal Finance Manager Showcase](https://jeffjojerjonescatulay.github.io/project-docu-pages/pfm/index.html)**

## 🛠️ Setup & Running

This project is fully containerized using Docker. To get the entire system up and running, follow these steps:

### 1. Clone the Infrastructure Repository
Navigate to the `pfm-infra` directory (or clone the standalone [pfm-infra repository](https://github.com/JeffJojerJonesCatulay/pfm-infra.git)).

### 2. Configure Environment Variables
Create a `.env` file in the root of the `pfm-infra` directory. You can use the following dummy data as a template:

```env
# Database Credentials
MYSQL_ROOT_PASSWORD=your_root_password
MYSQL_DATABASE=pfm_db
MYSQL_USER=pfm_user
MYSQL_PASSWORD=pfm_password

# API Configuration
API_IMAGE_TAG=v1.0.1
API_PORT=9010
API_SECRET=ThisIsMySuperSecureSecretKeyThatMustBeLongEnoughForJWTManualProccessing

# Web Configuration
WEB_IMAGE_TAG=v1.0.1
WEB_PORT=5173
VITE_PFM_BASE_URL=/api/v1.0.0/pfm/
```

> [!TIP]
> **API_SECRET** should be a long, random string (minimum **64 characters**) to ensure strong security for JWT signatures and to meet encryption requirements.

> [!NOTE]
> For the latest available image tags, please refer to my [Docker Hub Repositories](https://hub.docker.com/repositories/jeffjojerjonescatulay).

### 3. Run with Docker Compose
From the `pfm-infra` directory, execute the following command to start all services (database, API, and web app):

```bash
docker compose up -d
```

The system will be accessible at:
- **Frontend:** `http://localhost:5173`
- **Backend API:** `http://localhost:9010`

## 🏠 Personal Deployment Note

For personal use and cost-optimization, the production-like environment for this project is hosted directly on a **local machine** (personal laptop). Public access is managed through a **secure tunnel**, which routes traffic to the local containers. This setup allows for a fully functional, live demo environment while keeping infrastructure costs to a minimum.

## Project Structure

This repository acts as the **main hub**. Other repositories will contain modular components such as:

- **Frontend UI** – Dashboard and visualization tools
- **Backend Services** – APIs for data storage and processing

Links to these repositories will be added as development progresses.

PFM-Database: [Repo](https://github.com/JeffJojerJonesCatulay/pfm-database.git) | [Pages](https://jeffjojerjonescatulay.github.io/pfm-database/)

![DB](./docs/images/db.png)

PFM-Rest-API: [Repo](https://github.com/JeffJojerJonesCatulay/pfm-springboot-rest-api.git) | [Pages](https://jeffjojerjonescatulay.github.io/pfm-springboot-rest-api/)

![API](./docs/images/api.png)

PFM-Web: [Repo](https://github.com/JeffJojerJonesCatulay/pfm-web.git) | [Pages](https://jeffjojerjonescatulay.github.io/pfm-web/)

![Web](./docs/images/web.png)

PFM-Test: [Repo](https://github.com/JeffJojerJonesCatulay/pfm-test.git) | [Pages](https://jeffjojerjonescatulay.github.io/pfm-test/)

![Test](./docs/images/test.png)

PFM-Infra: [Repo](https://github.com/JeffJojerJonesCatulay/pfm-infra.git) | [Pages](https://jeffjojerjonescatulay.github.io/pfm-infra/)

![Infra](./docs/images/infra.png)

---
*Note: Images used in this project were generated using Microsoft Copilot.*

### 💡 Author's Note

This project was developed as a showcase of **Generative AI, Prompt Engineering, and Agentic Development**. 

While I possess basic knowledge of web technologies, I am not an expert in **React, TypeScript, or UI Design**. The entire codebase, including the REST API and the Web Application, was architected and implemented using **Google Antigravity**. This project stands as a testament to the power of agentic AI in modern software development.



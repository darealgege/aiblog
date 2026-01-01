# 🤖 AI Blog Engine 1.0

[![PayPal Donate Button](https://hungaryvfr.hu/images/paypal-donate-button-2.png)](https://www.paypal.com/ncp/payment/KUM7TUZW4CNPN)

**AI Blog Engine 2.0** is a high-performance, self-hosted PHP blogging platform designed for full automation and SEO dominance. It leverages advanced AI models and deep research APIs to create human-like, data-driven content with minimal human intervention.

---

## 🌟 Key Features

### 🧠 Advanced AI Logic
- **Deep Research**: Integrates **Brave Search** and **Perplexity AI** to gather real-time data and facts before writing.
- **Multi-Model Strategy**: Uses a tiered approach (GPT-4o-mini for drafting, GPT-4o for final polishing) to balance cost and quality.
- **Trend Analysis**: Automatically identifies trending topics to keep your content relevant and competitive.
- **Automated Media**: Extracts high-quality images and YouTube videos from source materials to enrich posts.

### 🚀 SEO & Performance
- **Automated SEO**: Generates meta titles, descriptions, and OpenGraph tags automatically.
- **Schema.org Integration**: Built-in JSON-LD for Articles, Breadcrumbs, and Blog structures.
- **Multilingual Support**: Seamlessly handles content in **Hungarian (HU)**, **English (EN)**, and **German (DE)** with correct `hreflang` implementation.
- **Internal Linking**: Smart "Related Posts" and topic-hub architecture to improve crawlability.

### 🛠️ Management & Analytics
- **Powerful Admin Panel**: Total control over topics, sources, and generated content.
- **Task Scheduler (Agent)**: A core background worker that handles crawling, research, and generation autonomously.
- **Visitor Tracking**: Built-in analytics for page views and visitor behavior without heavy third-party scripts.
- **Comment Moderation**: AI-assisted filtering to keep your community discussions clean and relevant.

---

## 💻 Tech Stack

- **Backend**: PHP 7.4+ (Compatible with PHP 8.x)
- **Database**: MySQL / MariaDB
- **Frontend**: Vanilla CSS & JavaScript (Modern, lightweight, and fast)
- **APIs**: OpenAI, Brave Search, Perplexity AI
- **UI**: Premium design system with **Dark/Light mode** support.

---

## 🏗️ Installation & Setup

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/darealgege/aiblog.git
   cd aiblog
   ```

2. **Configure Database**:
   Create a MySQL database and import the provided `.sql` schema if available (or use the installer).

3. **Environment Variables**:
   Create a `.env` file in the root directory (use `.env.example` as a template):
   ```ini
   DB_HOST=localhost
   DB_NAME=your_db_name
   DB_USER=your_db_user
   DB_PASS=your_db_password
   AI_API_KEY=your_openai_key
   PERPLEXITY_API_KEY=your_perplexity_key
   BRAVE_API_KEY=your_brave_key
   SITE_URL=https://yourdomain.com
   ```

4. **Run Setup Script**:
   Navigate to `https://yourdomain.com/install/setup.php` in your browser to finalize the installation.

---

## 🤖 The AI Agent (Automation)

The project relies on a background worker (`core/Agent.php`) to perform autonomous tasks.

### Running the Agent
You can trigger the agent manually from the Admin Dashboard or set up a Cron Job for full automation:

**Cron Job Example (every 15 minutes):**
```bash
*/15 * * * * php /path/to/your/project/cron/agent_worker.php
```

---

## 🔒 Security

- **Security Headers**: Built-in protection against XSS, Clickjacking, and MIME-sniffing.
- **Session Protection**: Secure session handling with CSRF prevention.
- **Input Sanitization**: Strict filtering for all user and AI-generated inputs.

---

## ☕ Support the Project

If you find this project useful and want to support its development, consider a donation:

[![PayPal Donate Button](https://hungaryvfr.hu/images/paypal-donate-button-2.png)](https://www.paypal.com/ncp/payment/KUM7TUZW4CNPN)

---

## 📄 License

This project is licensed under the MIT License. Developed with ❤️ by [darealgege](https://github.com/darealgege).


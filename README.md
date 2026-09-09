<div align="center">

# 🚢 FreightQuote AI

### Agentic AI for Maritime Freight Intelligence

<p>
  <i>Intelligent decision support for modern ocean-freight operations</i>
</p>

---

<table>
<tr>
<td align="center">🤖<br><b>9 AI Agents</b><br><sub>Specialised freight intelligence</sub></td>
<td align="center">🧠<br><b>AI Copilot</b><br><sub>Grounded responses</sub></td>
<td align="center">📊<br><b>ML Intelligence</b><br><sub>Prediction & analysis</sub></td>
</tr>

<tr>
<td align="center">🔎<br><b>RAG</b><br><sub>PDF knowledge retrieval</sub></td>
<td align="center">🌦️<br><b>Live Weather</b><br><sub>Port & route risk</sub></td>
<td align="center">🔐<br><b>Secure Access</b><br><sub>JWT + RBAC + OTP</sub></td>
</tr>
</table>

<br>

**Route Intelligence** &nbsp;→&nbsp;
**Dynamic Pricing** &nbsp;→&nbsp;
**Carrier Analysis** &nbsp;→&nbsp;
**Weather Risk**

**Margin Optimization** &nbsp;→&nbsp;
**Customs** &nbsp;→&nbsp;
**Documents** &nbsp;→&nbsp;
**Translation** &nbsp;→&nbsp;
**RAG**

<br>

<sub>
Infosys Springboard Internship · Batch 1
</sub>

</div>
<div align="center">


---

FreightQuote AI is an agentic decision-support platform for maritime freight operations. It brings together **route intelligence, freight pricing, carrier performance, weather risk, customs and tariff support, document processing, multilingual translation, and PDF-based knowledge retrieval** in a single platform.

The platform combines **9 specialised AI agents, machine-learning models, RAG-based retrieval, live weather information, SQLite, and a grounded AI Copilot** to support faster and more informed freight decisions.

**Route & Port → Pricing → Carrier → Weather → Margin → Customs → Documents → Translation → RAG**

---


## ✨ What the Platform Provides

| Capability | What it does |
|---|---|
| 🤖 **9 Specialised Agents** | Handles different parts of the maritime freight workflow |
| 🧠 **Grounded AI Copilot** | Answers operational questions using retrieved or computed information |
| 💰 **Freight Pricing** | Calculates and analyses freight quotes and rates |
| 🗺️ **Route Intelligence** | Supports route optimization and port/route analysis |
| 🚢 **Carrier Intelligence** | Evaluates carrier performance, reliability and capacity |
| 🌦️ **Weather Risk** | Uses live weather information for port and route-risk analysis |
| 📈 **Margin & Yield Optimization** | Supports freight profitability and margin decisions |
| 📋 **Customs & Tariff Intelligence** | Supports customs, HS-code and tariff-related decisions |
| 📄 **OCR & Shipping Documents** | Processes freight documents and Bill of Lading information |
| 🌐 **Multilingual Translation** | Translates maritime documents and policies |
| 📚 **Custom PDF RAG** | Retrieves answers from uploaded PDF knowledge sources |
| 🔐 **Authentication & RBAC** | Provides secure login, role-based access and session handling |
| 👨‍💼 **Admin Dashboard** | Provides user management, ML metrics and audit visibility |

---

# 📑 Table of Contents

- [Program & Team](#-program--team)
- [Project Overview](#-project-overview)
- [Objectives](#-objectives)
- [System Architecture](#-system-architecture)
- [The 9 Specialised Agents](#-the-9-specialised-agents)
- [Technology Stack](#-technology-stack)
- [AI Copilot](#-ai-copilot)
- [Authentication & Security](#-authentication--security)
- [Admin Dashboard](#-admin-dashboard)
- [Machine Learning](#-machine-learning)
- [RAG & Knowledge Retrieval](#-rag--knowledge-retrieval)
- [Weather Intelligence](#-weather-intelligence)
- [Document Processing & Translation](#-document-processing--translation)
- [Platform Intelligence Tools](#-platform-intelligence-tools)
- [Screenshots](#-screenshots)
- [Project Structure](#-project-structure)
- [Installation & Run](#-installation--run)
- [Environment Variables](#-environment-variables)
- [Testing & Validation](#-testing--validation)
- [Challenges & Learnings](#-challenges--learnings)
- [Future Scope](#-future-scope)
- [Acknowledgements](#-acknowledgements)

---

# 👥 Program & Team

### Infosys Springboard Internship — Batch 1

**Project:** FreightQuote AI

### Team

| # | Team Member | Primary Contribution |
|---|---|---|
| 01 | **Tharani Mahasamudram** | Agent validation & functional testing · Multi-agent execution verification · ML model/output checking · Architecture review · PPT and quality support |
| 02 | **Samathasri Kamireddy** | Authentication & security features · OTP and password recovery · JWT/session handling · Logout functionality · Presentation/PPT support |
| 03 | **Kavya Shree** | AI Copilot & RAG integration · Natural-language query handling · Grounded response generation · LLM integration · Copilot testing |
| 04 | **Yuvanesh V** | Dynamic Freight Pricing · Route & Maritime Fuel Efficiency · Carrier Performance & Capacity Intelligence · Weather Risk & Storm Telemetry · Module integration |
| 05 | **Sravya Nanda** | Customs, Tariff & Regulatory Intelligence · HS Code support · Digital Bill of Lading & OCR · Document processing · Compliance validation |
| 06 | **Sai Laghuvar** | Freight Margin & Yield Optimization · Anomaly & Risk Scanner · Alerts & Incident handling · Knowledge Graph · Digital Twin · Platform testing |

> FreightQuote AI was developed collaboratively, with the team contributing across AI development, agent validation, integration, testing, documentation and presentation.

---

# 🧭 Project Overview

## Problem Statement

Maritime freight operations require decisions across several areas at the same time, including:

- Freight pricing
- Route selection
- Port conditions
- Carrier performance
- Weather and storm risk
- Customs and tariffs
- Shipping documentation
- Translation
- Knowledge retrieval

When this information is distributed across different tools and datasets, decision-making becomes slower and more difficult.

### Our Approach

FreightQuote AI brings these capabilities together through a single agentic platform where specialised agents handle individual operational tasks and the AI Copilot provides a unified interface for querying the available information.

---

# 🎯 Objectives

The main objectives of FreightQuote AI are to:

1. Automate repetitive maritime freight analysis.
2. Provide dynamic freight pricing and quote intelligence.
3. Support route and port decision-making.
4. Analyse carrier reliability and capacity.
5. Identify weather and storm-related risks.
6. Support freight margin and yield decisions.
7. Assist with customs, tariffs and regulatory information.
8. Process shipping documents using OCR.
9. Provide multilingual maritime-document translation.
10. Enable question answering over custom PDF documents using RAG.
11. Provide grounded AI responses instead of unsupported generated facts.
12. Provide role-based access and administrative controls.
13. Bring multiple operational capabilities together in one interface.

---

# 🏗️ System Architecture

The platform is organised around authentication, multi-agent orchestration, data/model services and grounded response generation.

### Architecture Flow

```text
User
  ↓
Authentication & RBAC
  ↓
FreightQuote AI Platform
  ↓
Multi-Agent Orchestration
  ↓
SQLite / FAISS / ML Models / APIs
  ↓
Qwen 2.5 LLM
  ↓
Grounded Final Response
```

### Architecture Diagram

![FreightQuote AI System Architecture](docs/architecture-diagram.png)

The architecture separates the user-facing application from the specialised agents, data sources, retrieval components and AI generation layer.

---

# 🤖 The 9 Specialised Agents

| # | Agent | Main Functions |
|---|---|---|
| **1** | 🚢 **Port & Route Intelligence** | • Route optimization<br>• Port analysis<br>• Port congestion insights<br>• Distance and route evaluation<br>• Route-risk assessment |
| **2** | 💰 **Dynamic Freight Pricing** | • Freight quote calculation<br>• Spot-rate analysis<br>• Base cost estimation<br>• Final quote calculation<br>• Pricing and margin analysis |
| **3** | 📊 **Carrier Performance & Capacity** | • Carrier performance analysis<br>• Reliability scoring<br>• Capacity intelligence<br>• Carrier comparison<br>• Delay/risk insights |
| **4** | 🌦️ **Weather Risk & Storm Telemetry** | • Live weather monitoring<br>• Port weather analysis<br>• Storm-risk assessment<br>• Weather-based route risk<br>• Safety insights |
| **5** | 📈 **Dynamic Margin & Yield Optimizer** | • Freight margin analysis<br>• Profitability calculation<br>• Margin prediction<br>• Yield optimization<br>• Margin sensitivity analysis |
| **6** | 📋 **Customs & HS Code Compliance** | • Customs information<br>• HS Code support<br>• Tariff analysis<br>• Duty estimation<br>• Regulatory/compliance insights |
| **7** | 📄 **Quote & Bill of Lading Docs** | • Freight quote generation<br>• Bill of Lading processing<br>• Shipping-document handling<br>• OCR/document extraction<br>• Document validation |
| **8** | 🌐 **Document & Policy Translation** | • Multilingual translation<br>• Maritime document translation<br>• Customs/policy translation<br>• Multiple-language support<br>• NLLB-200 based translation |
| **9** | 📚 **Custom PDF Knowledge RAG** | • PDF document ingestion<br>• Text extraction<br>• FAISS vector search<br>• Relevant knowledge retrieval<br>• Grounded question answering |

### Agent Design

Each agent is focused on a specific operational area. This allows the platform to select the appropriate data, calculation, model or retrieval mechanism instead of depending on one general-purpose process for every request.

---

# 🛠️ Technology Stack

| Layer | Technologies |
|---|---|
| **Frontend / UI** | Streamlit |
| **Backend / Application Logic** | Python |
| **API Layer** | FastAPI components where required |
| **LLM** | Qwen2.5-3B-Instruct |
| **LLM Fallback** | Qwen2.5-1.5B-Instruct |
| **Vector Search** | FAISS |
| **Embeddings** | Sentence Transformers |
| **Database** | SQLite |
| **Weather API** | Open-Meteo REST API |
| **Translation** | NLLB-200 |
| **Machine Learning** | scikit-learn |
| **Visualisation** | Plotly / Streamlit visualisation |
| **Authentication** | PyJWT / bcrypt |
| **Tunnelling** | ngrok / Cloudflare Tunnel |
| **Development** | Google Colab, Kaggle datasets |
| **Documents** | PDF / OCR processing |
| **Reporting** | ReportLab / PDF generation |

---

# 🧠 AI Copilot

The AI Copilot acts as the main natural-language interface to FreightQuote AI.

Instead of manually navigating through every agent, a user can ask an operational question and the Copilot determines how to obtain the required information.

## Answer Pipeline

```text
User Question
     ↓
classify_intent()
     ↓
Identify shipment / pricing / weather /
customs / carrier intent
     ↓
run_grounded_query()
     ↓
SQL / route solver / relevant agent
     ↓
execute_tool() → RAG fallback
     ↓
generate_grounded_answer()
     ↓
Qwen2.5-3B
     ↓
Final grounded response
```

### Grounding Principle

The Copilot is designed to prioritise:

- Retrieved knowledge
- SQL/database results
- Computed results
- Agent outputs
- RAG evidence

It should not invent numbers, metrics or sources when supporting evidence is unavailable.

### Multilingual Support

The platform also supports multilingual interaction through the translation layer, allowing maritime information and documents to be handled across multiple languages.

---

# 🔐 Authentication & Security

FreightQuote AI includes authentication and role-based access control.

### Login Flow

```text
Signup / Login
      ↓
Forgot Password
      ↓
OTP Verification
      ↓
Security Question
      ↓
Role-Scoped Session
```

### Security Components

- Password hashing with bcrypt
- JWT-based session handling
- OTP-based verification/recovery
- Security-question support
- Logout functionality
- Role-based access control
- Admin-only dashboard access
- Session-aware navigation

### RBAC Roles

| Role | Access |
|---|---|
| 👑 **Admin** | Full platform access including Admin Dashboard |
| 🚢 **Freight Broker / Ops Manager** | Operational agents and AI Copilot |
| 📦 **Dispatcher** | AI Copilot and selected operational agents |
| 👤 **Customer / Client** | AI Copilot and quote-related functionality |

---

# 👨‍💼 Admin Dashboard

The Admin Dashboard provides a central view for platform administration.

### Main Areas

**User Management**
- User/account management
- Role management
- Account controls

**ML Model Performance Ledger**
- Agent/model performance information
- Accuracy/F1 tracking where applicable
- Benchmark-related metrics

**Chat & Audit Trail**
- AI Copilot conversation history
- Audit visibility
- Operational review

The dashboard is designed to provide administrators with visibility into both users and system performance.

---

# 📊 Machine Learning

Machine-learning models are used across different operational agents depending on the task.

### Algorithms Used / Evaluated

- Random Forest
- Gradient Boosting
- Extra Trees
- Decision Tree
- Logistic Regression
- Ridge Regression
- AdaBoost
- K-Nearest Neighbours
- Support Vector Machine
- Multi-Layer Perceptron

### Example Model Mapping

| Agent | Example ML Application |
|---|---|
| Dynamic Freight Pricing | Freight-price prediction |
| Carrier Performance | Reliability/classification analysis |
| Weather Risk | Risk classification |
| Customs | Classification support |
| Freight Margin | Margin/profit prediction |

Model outputs are integrated into the agent workflow rather than being presented as isolated ML experiments.

---

# 📚 RAG & Knowledge Retrieval

The Custom PDF Knowledge Agent provides document-based retrieval.

### RAG Pipeline

```text
PDF Upload
    ↓
Text Extraction
    ↓
Chunking
    ↓
Sentence-Transformer Embeddings
    ↓
FAISS Vector Index
    ↓
Similarity Search
    ↓
Relevant Chunks
    ↓
Grounded Answer
```

### Why RAG?

RAG allows the Copilot to answer questions using the content of uploaded documents instead of relying only on the language model's internal knowledge.

This is especially useful for:

- Maritime SOPs
- Customs documents
- Policies
- Contracts
- Operational manuals
- Freight-related PDFs

---

# 🌦️ Weather Intelligence

The Weather Risk agent uses live weather information to support maritime risk analysis.

The weather layer can provide information such as:

- Weather conditions
- Wind conditions
- Wave-related risk indicators where available
- Port weather information
- Storm-risk signals
- Route-risk context

The system uses weather information as supporting context for operational decisions.

---

# 📄 Document Processing & Translation

## OCR & Shipping Documents

The document-processing capabilities support:

- Freight quote documents
- Bill of Lading documents
- OCR-based extraction
- Shipping-document information
- Document validation

## Multilingual Translation

The translation agent uses **NLLB-200** for multilingual document and policy translation.

It supports the broader platform by allowing users to work with maritime information across languages.

---

# 🧩 Platform Intelligence Tools

Beyond the nine specialised agents, the platform includes shared intelligence tools available through the role-based interface.

| Tool | Purpose |
|---|---|
| 🔔 **Notifications** | Unified operational incident and alert feed |
| 🕸️ **Knowledge Graph** | Relationship-based exploration of ports, routes and carriers |
| 🌐 **Digital Twin** | Network-level simulation for stress testing and decision support |
| 🎯 **Anomaly Scanner** | Detects unusual operational patterns |
| 🗄️ **Data Feed Center** | Operational data export and review |

### Digital Twin — Why We Use It

A **Digital Twin** is a virtual representation of a real-world system.

In FreightQuote AI, it can be used conceptually to simulate maritime-network conditions and test scenarios before making operational decisions.

For example, a team could examine how changes in routes, pricing or network conditions might affect operations.

---

# 📸 Screenshots

The repository includes selected screenshots demonstrating the platform.

## 🔐 Login

![FreightQuote AI Login](docs/screenshots/login.jpeg)

## 🤖 Agent Interface

![Agent Example](docs/screenshots/agent-example.jpeg)

## 🧠 AI Copilot

![AI Copilot](docs/screenshots/copilot-chat.jpeg)

## 👨‍💼 Admin Dashboard

![Admin Dashboard](docs/screenshots/admin_dashboard.jpeg)

## 🏗️ Architecture

![Architecture Diagram](docs/architecture-diagram.png)

---

# 🎥 Demo

A recorded demonstration is included in the repository:

[`docs/demo.mp4`](docs/demo.mp4)

The demo covers the integrated FreightQuote AI platform and its major workflows.

---

# 📁 Project Structure

```text
FreightQuote-AI/
│
├── app.py
├── auth.py
├── db.py
├── admin_dash.py
├── train_ml.py
├── llm_engine.py
├── config.py
├── notifications.py
├── ui_theme.py
├── ui_enhancements.py
├── weather_context.py
├── seed_data.py
├── agent2_freight.py
├── agent3_freight.py
│
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .env.example
├── .gitignore
├── LICENSE
├── README.md
│
├── docs/
│   ├── architecture-diagram.png
│   ├── demo.mp4
│   │
│   └── screenshots/
│       ├── login.jpeg
│       ├── agent-example.jpeg
│       ├── copilot-chat.jpeg
│       └── admin_dashboard.jpeg
│
├── Milestone4/
└── Milestone_3/
```

> Additional agent/model files may be present depending on the final integrated repository version.

---

# 🚀 Installation & Run

## 1. Clone the Repository

```bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd FreightQuote-AI
```

## 2. Create a Virtual Environment

### Windows

```bash
python -m venv venv
venv\Scripts\activate
```

### Linux / macOS

```bash
python3 -m venv venv
source venv/bin/activate
```

## 3. Install Dependencies

```bash
pip install -r requirements.txt
```

## 4. Configure Environment Variables

Create a `.env` file based on `.env.example`.

```bash
cp .env.example .env
```

On Windows, create the `.env` file manually if required.

## 5. Run the Application

```bash
streamlit run app.py
```

The application will provide a local Streamlit URL in the terminal.

---

# 🔑 Environment Variables

The project uses environment variables for credentials and configuration.

Typical configuration includes:

```env
HF_TOKEN=
KAGGLE_USERNAME=
KAGGLE_KEY=
JWT_SECRET_KEY=
NGROK_AUTHTOKEN=

ADMIN_EMAIL_ID=
ADMIN_PASSWORD=

EMAIL_ID=
EMAIL_PASSWORD=
```

### ⚠️ Security

**Never commit real credentials, API keys, passwords, OTPs or tokens to GitHub.**

Use `.env.example` only for variable names/placeholders.

The `.gitignore` file should exclude sensitive environment files such as:

```text
.env
```

---

# 🧪 Testing & Validation

The integrated platform was checked across the major functional areas.

### Validation Areas

- Login and authentication
- Role-based access
- Agent navigation
- Agent execution
- Pricing calculations
- Route intelligence
- Carrier analysis
- Weather information
- Margin analysis
- Customs functionality
- Document processing
- Translation
- PDF/RAG retrieval
- AI Copilot responses
- Admin Dashboard
- Database operations
- UI navigation
- Error handling

### Agent Validation

Each specialised agent should be checked for:

1. Correct page loading.
2. Correct input handling.
3. Successful execution.
4. Expected output.
5. Model/database/API availability.
6. Error handling.
7. Integration with the overall platform.

---

# 📈 Results & Impact

The project presentation highlights the intended operational impact of the integrated platform:

| Impact Area | Reported Project Impact |
|---|---:|
| ⚡ Faster Information Retrieval | **70%** |
| 📄 Reduction in Manual Documentation Effort | **65%** |
| 🤖 Automation of Routine Freight Analysis | **80%** |

These improvements are associated with combining AI-powered retrieval, OCR, semantic search, document processing and specialised freight agents into a single workflow.

### Overall Benefits

**Higher Efficiency · Lower Costs · Better Visibility**

---

# 🧩 Challenges & Learnings

During development and integration, several practical challenges required attention.

### 1. Keeping AI Responses Grounded

The Copilot needed to avoid producing unsupported numbers or information.

The solution was to prioritise retrieved SQL results, computed outputs and RAG evidence and make the response generation layer aware of missing evidence.

### 2. Live Weather API Reliability

Real-time weather APIs can occasionally experience timeouts or rate limitations.

The system therefore needs graceful handling when live weather information is temporarily unavailable.

### 3. SQLite Concurrency

Multiple agents may access the database during the same application workflow.

SQLite connection handling and database operations therefore required careful validation to avoid locking or connection-related issues.

### 4. Multi-Agent Integration

Integrating nine different operational agents into a single interface required consistent navigation, inputs, outputs and error handling.

### Key Learning

The project provided practical experience in combining **AI, RAG, machine learning, APIs, databases, authentication and UI development** into one integrated application rather than developing each technology independently.

---

# 🔮 Future Scope

The platform can be extended further in several directions:

### 1. ☁️ Cloud-Native Scaling

Deploy the platform using containerised cloud infrastructure for scalable multi-user operations.

### 2. 🚢 Real Carrier API Integrations

Replace simulated/static carrier data with live carrier APIs and rate feeds.

### 3. 🗄️ PostgreSQL Migration

Move from SQLite to PostgreSQL for stronger concurrent multi-user production workloads.

### 4. 🔔 Mobile Push Alerts

Provide real-time incident and customs-hold notifications through a companion mobile application.

---

# 🏆 Key Takeaway

FreightQuote AI demonstrates how an **agentic AI architecture** can bring multiple maritime freight activities into one decision-support platform.

Instead of treating pricing, routing, weather, carriers, customs, documents and knowledge retrieval as separate systems, the platform connects them through specialised agents and a grounded AI Copilot.

> **One platform. Nine specialised agents. Grounded intelligence for maritime freight decisions.**

---

# 🙏 Acknowledgements

We would like to express our sincere gratitude to **Infosys Springboard** for providing the internship platform and learning opportunity.

We are especially thankful to our mentor,

### **Mohamed Sipli M**

for the guidance, feedback, technical direction and continuous support throughout the development and evaluation of this project.

**Thank you, Sir, for your guidance and support throughout the project.**

---

## 👥 FreightQuote AI Team

**Tharani Mahasamudram · Samathasri Kamireddy · Kavya Shree · Yuvanesh V · Sravya Nanda · Sai Laghuvar**

---

### 📌 Project Information

**Program:** Infosys Springboard Internship — Batch 1  
**Project:** FreightQuote AI  
**Domain:** Agentic AI for Maritime Freight  
**Focus:** Freight Pricing · Route Optimization · Risk Intelligence · Documentation · RAG · AI Copilot
## 📸 Screenshots

The repository includes selected screenshots demonstrating the platform.

### Login & Access
<img width="1262" height="698" alt="Screenshot 2026-08-19 130930" src="https://github.com/user-attachments/assets/0917462a-8c23-47b7-b711-86fbcc5adde4" />

*Secure sign-in screen with role-based demo credentials.*

### Admin Dashboard
<img width="1258" height="585" alt="Screenshot 2026-08-19 130953" src="https://github.com/user-attachments/assets/7f24c56a-de90-448c-9d11-b489c348e787" />

*Command-center overview of shipments, quotes, and platform-wide KPIs.*

### AI Copilot
<img width="1262" height="594" alt="Screenshot 2026-08-19 131010" src="https://github.com/user-attachments/assets/5f73b908-397d-425f-a45f-7f8b8962271a" />

*Grounded chat assistant answering questions using live freight data.*

### Route Optimization (Agent 1)
<img width="1263" height="590" alt="Screenshot 2026-08-19 131023" src="https://github.com/user-attachments/assets/51380aa1-8f99-4cf8-975e-f8720bc27264" />

*Interactive port-to-port route mapping and optimization analysis.*

### Dynamic Freight Pricing (Agent 2)
<img width="1262" height="579" alt="Screenshot 2026-08-19 131038" src="https://github.com/user-attachments/assets/e7d1ba44-d9d0-48da-880c-5cae97bcdbcc" />

*Real-time dynamic pricing engine for freight quotes.*

### Carrier Performance (Agent 3)
<img width="1264" height="584" alt="Screenshot 2026-08-19 131052" src="https://github.com/user-attachments/assets/c7269898-d765-47a5-96f8-d810622d7486" />

*Carrier capacity, reliability, and performance analytics.*

### Weather & Freight Risk (Agent 4)
<img width="1262" height="585" alt="Screenshot 2026-08-19 131106" src="https://github.com/user-attachments/assets/90cfdbab-27f3-4bb2-af4d-632fe98b3b3b" />

*Live port weather overlays and shipment risk scoring.*

### Margin Predictor (Agent 5)
<img width="1259" height="585" alt="Screenshot 2026-08-19 131121" src="https://github.com/user-attachments/assets/6d0a97b1-65b2-4074-a50f-bc767077ba8a" />

*Predicted yield and margin outlook across active shipments.*

### Customs & Tariffs (Agent 6)
<img width="1263" height="587" alt="Screenshot 2026-08-19 131134" src="https://github.com/user-attachments/assets/58a2df26-f861-4ee4-99a4-07a9f08640f3" />

*Customs, tax, and compliance guidance for cross-border shipments.*

### Digital Bill of Lading (Agent 7)
<img width="1260" height="581" alt="Screenshot 2026-08-19 131147" src="https://github.com/user-attachments/assets/8900fb18-f54a-46e6-9088-fc98dcde70a8" />

*Automated generation and management of shipping documents.*

### Alerts & Translation (Agent 8)
<img width="1263" height="588" alt="Screenshot 2026-08-19 131201" src="https://github.com/user-attachments/assets/3d6c519f-bda3-4404-b964-008038b59113" />

*Real-time incident alerts alongside 20+ language translation support.*

### PDF SOP / RAG Studio (Agent 9)
<img width="1260" height="587" alt="Screenshot 2026-08-19 131213" src="https://github.com/user-attachments/assets/d5a4eaea-7db2-4df9-8c16-b4026508be9e" />

*Upload and query customs/SOP PDFs using retrieval-augmented search.*

### Anomaly Scanner
<img width="1259" height="588" alt="Screenshot 2026-08-19 131233" src="https://github.com/user-attachments/assets/db8666ae-93d3-4df1-b8e9-fd62a33e2823" />

*Isolation Forest–based detection of anomalies across shipments and ports.*

### Digital Twin Simulation
<img width="1259" height="588" alt="Screenshot 2026-08-19 131250" src="https://github.com/user-attachments/assets/cd4bd8b6-1244-40ca-9e4a-5619f05a4cf5" />

*Monte Carlo trade-stress simulation of the global freight network.*

### Knowledge Graph
<img width="1264" height="584" alt="Screenshot 2026-08-19 131306" src="https://github.com/user-attachments/assets/ea4ff774-e2b3-4c10-93d1-5079fc43b5a4" />

*Interactive graph linking ports, carriers, shipments, and documents.*

### Data Feed Center
<img width="1264" height="585" alt="Screenshot 2026-08-19 131320" src="https://github.com/user-attachments/assets/f60fb7fe-1706-450a-9774-876ccb993f43" />

*Manual and bulk CSV data ingestion into the live database.*

---

📁 Project Structure
text
FreightQuote-AI/
│
├── app.py
├── auth.py
├── db.py
├── admin_dash.py
├── train_ml.py
├── llm_engine.py
├── config.py
├── notifications.py
├── ui_theme.py
├── ui_enhancements.py
├── weather_context.py
├── seed_data.py
├── agent2_freight.py
├── agent3_freight.py
│
├── requirements.txt
├── Dockerfile
├── docker-compose.yml
├── .env.example
├── .gitignore
├── LICENSE
├── README.md
│
├── docs/
│   ├── architecture-diagram.png
│   ├── demo.mp4
│   │
│   └── screenshots/
│       ├── login.jpeg
│       ├── agent-example.jpeg
│       ├── copilot-chat.jpeg
│       └── admin_dashboard.jpeg
│
├── Milestone4/
└── Milestone_3/

Additional agent/model files may be present depending on the final integrated repository version.

🚀 Installation & Run
1. Clone the Repository
bash
git clone <YOUR_GITHUB_REPOSITORY_URL>
cd FreightQuote-AI
2. Create a Virtual Environment
Windows
bash
python -m venv venv
venv\Scripts\activate
Linux / macOS
bash
python3 -m venv venv
source venv/bin/activate
3. Install Dependencies
bash
pip install -r requirements.txt
4. Configure Environment Variables

Create a .env file based on .env.example.

bash
cp .env.example .env

On Windows, create the .env file manually if required.

5. Run the Application
bash
streamlit run app.py

The application will provide a local Streamlit URL in the terminal.

🔑 Environment Variables

The project uses environment variables for credentials and configuration.

Typical configuration includes:

env
HF_TOKEN=
KAGGLE_USERNAME=
KAGGLE_KEY=
JWT_SECRET_KEY=
NGROK_AUTHTOKEN=

ADMIN_EMAIL_ID=
ADMIN_PASSWORD=

EMAIL_ID=
EMAIL_PASSWORD=
⚠️ Security

Never commit real credentials, API keys, passwords, OTPs or tokens to GitHub.

Use .env.example only for variable names/placeholders.

The .gitignore file should exclude sensitive environment files such as:

text
.env
🧪 Testing & Validation

The integrated platform was checked across the major functional areas.

Validation Areas
Login and authentication
Role-based access
Agent navigation
Agent execution
Pricing calculations
Route intelligence
Carrier analysis
Weather information
Margin analysis
Customs functionality
Document processing
Translation
PDF/RAG retrieval
AI Copilot responses
Admin Dashboard
Database operations
UI navigation
Error handling
Agent Validation

Each specialised agent should be checked for:

Correct page loading.
Correct input handling.
Successful execution.
Expected output.
Model/database/API availability.
Error handling.
Integration with the overall platform.
📈 Results & Impact

The project presentation highlights the intended operational impact of the integrated platform:

Impact Area	Reported Project Impact
⚡ Faster Information Retrieval	70%
📄 Reduction in Manual Documentation Effort	65%
🤖 Automation of Routine Freight Analysis	80%

These improvements are associated with combining AI-powered retrieval, OCR, semantic search, document processing and specialised freight agents into a single workflow.

Overall Benefits

Higher Efficiency · Lower Costs · Better Visibility

🧩 Challenges & Learnings

During development and integration, several practical challenges required attention.

1. Keeping AI Responses Grounded

The Copilot needed to avoid producing unsupported numbers or information.

The solution was to prioritise retrieved SQL results, computed outputs and RAG evidence and make the response generation layer aware of missing evidence.

2. Live Weather API Reliability

Real-time weather APIs can occasionally experience timeouts or rate limitations.

The system therefore needs graceful handling when live weather information is temporarily unavailable.

3. SQLite Concurrency

Multiple agents may access the database during the same application workflow.

SQLite connection handling and database operations therefore required careful validation to avoid locking or connection-related issues.

4. Multi-Agent Integration

Integrating nine different operational agents into a single interface required consistent navigation, inputs, outputs and error handling.

Key Learning

The project provided practical experience in combining AI, RAG, machine learning, APIs, databases, authentication and UI development into one integrated application rather than developing each technology independently.

🔮 Future Scope

The platform can be extended further in several directions:

1. ☁️ Cloud-Native Scaling

Deploy the platform using containerised cloud infrastructure for scalable multi-user operations.

2. 🚢 Real Carrier API Integrations

Replace simulated/static carrier data with live carrier APIs and rate feeds.

3. 🗄️ PostgreSQL Migration

Move from SQLite to PostgreSQL for stronger concurrent multi-user production workloads.

4. 🔔 Mobile Push Alerts

Provide real-time incident and customs-hold notifications through a companion mobile application.

🏆 Key Takeaway

FreightQuote AI demonstrates how an agentic AI architecture can bring multiple maritime freight activities into one decision-support platform.

Instead of treating pricing, routing, weather, carriers, customs, documents and knowledge retrieval as separate systems, the platform connects them through specialised agents and a grounded AI Copilot.

One platform. Nine specialised agents. Grounded intelligence for maritime freight decisions.

🙏 Acknowledgements

We would like to express our sincere gratitude to Infosys Springboard for providing the internship platform and learning opportunity.

We are especially thankful to our mentor,

Mohamed Sipli M

for the guidance, feedback, technical direction and continuous support throughout the development and evaluation of this project.

Thank you, Sir, for your guidance and support throughout the project.

👥 FreightQuote AI Team

Tharani Mahasamudram · Samathasri Kamireddy · Kavya Shree · Yuvanesh V · Sravya Nanda · Sai Laghuvar

📌 Project Information

Program: Infosys Springboard Internship 7.0 — Batch 1
Project: FreightQuote AI
Domain: Agentic AI for Maritime Freight
Focus: Freight Pricing · Route Optimization · Risk Intelligence · Documentation · RAG · AI Copilot

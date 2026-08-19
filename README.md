# Infosys_FreightQuote_AI
Infosys Springboard

## 📸 Application Screenshots

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

## 🌟 Milestone 4 Highlights

The major outcome of this milestone is the transition from separate project components to a **single integrated freight-intelligence platform**.

### Key takeaways

- Multiple AI agents can work within one application.
- Operational data and ML predictions are presented together.
- The AI Copilot can use structured database information and retrieved documents.
- RBAC provides different views for different users.
- RAG extends the system beyond structured database queries.
- Route, pricing, weather, carrier and customs analysis can be accessed from one interface.
- Supporting tools such as anomaly detection, digital twin simulation and knowledge graphs provide additional operational insight.

---

## 📖 Glossary (Simple Terms)

A few shipping terms used throughout this README, explained simply:

| Term | Simple Meaning |
|---|---|
| **BAF** | Bunker Adjustment Factor — an extra fee added to cover changing fuel prices |
| **TEU** | Twenty-foot Equivalent Unit — the standard way to measure how much a container can hold |
| **HS Code** | A code used worldwide to classify goods for customs purposes |
| **Dwell Time** | How long cargo sits at a port before it moves on |
| **Bill of Lading** | A shipping receipt/legal document showing what's being shipped and to whom |
| **RAG** | Retrieval-Augmented Generation — the AI looks up real documents before answering, instead of guessing |
| **RBAC** | Role-Based Access Control — different users see different features depending on their role |
| **OTP** | One-Time Password — a temporary code sent to your email to verify it's really you |

---

## ❓ Quick FAQ

**Q: Do I need a GPU to run this?**
A local LLM (Qwen) works best with a GPU, which is why the project is designed to run on Google Colab. It can fall back to a smaller model or CPU mode if no GPU is available, though responses will be slower.

**Q: Is the data real?**
No — ports, shipments, carriers, and customer data are generated for demo purposes. Only the live weather data (from Open-Meteo) is real-time.

**Q: Can the AI Copilot make up numbers?**
It's designed not to. The Copilot is instructed to answer only from data it can retrieve (the database or uploaded PDFs) and to say so clearly when it doesn't have enough information.

**Q: What happens if the 3B model can't load?**
The app automatically falls back to the smaller Qwen2.5-1.5B-Instruct model so the Copilot keeps working, just with slightly less detailed responses.

---

## ⚠️ Known Limitations & Future Scope

### Current Limitations
- Uses generated/synthetic data for most modules rather than live commercial freight data.
- SQLite is used for simplicity, which limits how many people can use the app at the same time.
- Designed as a single-organization demo rather than a multi-company production system.

### Possible Future Improvements
- Connect to real freight-rate and carrier APIs instead of demo data.
- Move to a more scalable database for multiple concurrent users.
- Add more languages and refine translation accuracy for maritime-specific terms.
- Expand the RAG knowledge base to update automatically from a shared document folder.

---

## 👥 Team Contribution

This project was developed collaboratively as part of the **Infosys Springboard Internship**. Each team member contributed to different modules of the Milestone 4 integrated platform.

| No. | Team Member | Contribution |
|---|---|---|
| **01** | **Yuvanesh** | Frontend development of the Streamlit application — dashboards, layout and UI wiring across all agent pages |
| **02** | **Nitya Balraj** | Backend development — agent modules, database (SQLite), authentication logic and LLM/API integration |
| **03** | **Kavyashree** | UI/UX design — visual styling, layout consistency and overall look-and-feel of the platform |
| **04** | **Sriharsha Thorupunuri** | GitHub repository management and README documentation; additional frontend development support |

---

# 🚀 Autonomous Data Pipeline & BI Agent

## 👥 Team Details

- **Team Name:** DataForge AI  
- **Members:**  
  - Member 1 
  - Member 2   
- **Domain Category:** Multi-Agent Systems    
- **Demo Video:** Sharepoint URL of your MVP demo  

---

## 🎯 Problem Statement

Data engineers and analysts spend significant time:

- Creating ETL pipelines  
- Generating analytics reports  
- Updating dashboards  
- Fixing broken data flows  

The process is manual, repetitive, and not self-improving.

---

## 💡 Solution Overview

We built a **Multi-Agent Autonomous Data Engineering System** that:

1. Creates data pipelines automatically  
2. Validates data quality  
3. Generates BI dashboards  
4. Self-improves based on failures and feedback  

The system uses specialized agents:

- 🛠 Pipeline Builder Agent  
- 📊 BI Report Agent  
- 🔍 Data Quality Agent  
- 🧠 Learning Agent  

Each agent communicates through a centralized orchestration layer.

---

## 🏗 Architecture

📁 Architecture Diagram: `/architecture/architecture.png`

### Components

- User Interface (Streamlit)  
- Orchestrator Agent  
- Pipeline Agent  
- BI Agent  
- Learning Agent  
- Vector Memory Store  
- External APIs (Azure OpenAI / Fabric / Synapse)  

### Flow

1. User submits dataset  
2. Orchestrator analyzes request  
3. Pipeline Agent generates ETL logic  
4. Data Quality Agent validates data  
5. BI Agent generates dashboard  
6. Learning Agent stores feedback  

---

## 🛠 Tech Stack

| Layer | Technology |
|-------|------------|
| Backend | Python |
| Frontend | Streamlit |
| AI Model | Azure OpenAI GPT-4 |
| Embeddings | text-embedding-3-large |
| Vector DB | FAISS |
| Database | PostgreSQL |
| Orchestration | LangGraph |

---

## 📂 Project Structure

```
autonomous-data-agent/
│
├── README.md              # Mandatory
├── requirements.txt       # Mandatory (or package.json for Node projects)
├── .env.example           # Mandatory
│
├── src/                   # Required if project contains source code
│   ├── main.py            # Clear entry point (mandatory)
│   ├── orchestrator.py
│   ├── agents/
│   │   ├── pipeline_agent.py
│   │   ├── bi_agent.py
│   │   ├── quality_agent.py
│   │   └── learning_agent.py
│   └── utils/
│       └── config.py
│
├── architecture/          # Mandatory (must include architecture diagram)
│   └── architecture.png
│
├── data/                  # Optional (if sample/test data is required)
│   └── sample_dataset.csv
```

---

### 🚨 Mandatory Files for All Submissions

The following files **must be present** in every submission:

- `README.md`
- `requirements.txt` (or `package.json` for Node projects)
- `.env.example`
-  Clear entry point inside `src/`
- `architecture/architecture.png` (or equivalent flow diagram)

All other folders (e.g., `data/`, `tests/`, `notebooks/`, etc.) may vary depending on the project.
Submissions missing mandatory files may not be evaluated.

---

## ⚙️ Setup Instructions

## 1️ Verify Required Software

- Programming Language: <Python / Node / Java / etc>
- Required Version: Exact Version
- Package Manager: <pip / npm / etc>

### 1️⃣ Clone Repository

```bash
git clone https://github.com/dataforge-ai/autonomous-data-agent
cd autonomous-data-agent
```

### 2️⃣ Create Virtual Environment

```bash
python -m venv venv
```

Activate:

**Windows**
```bash
venv\Scripts\activate
```

**Mac/Linux**
```bash
source venv/bin/activate
```

### 3️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

### 4️⃣ Configure Environment Variables

Create `.env` file from `.env.example`

Example:

```
OPENAI_API_KEY=your_key_here
DB_HOST=localhost
DB_USER=postgres
DB_PASSWORD=postgres
VECTOR_DB_PATH=./vector_store
```

---

## ▶️ Entry Point

Run the application:

```bash
streamlit run src/main.py
```

Application will start at:

```
http://localhost:8501
```

---

## 🔄 Application Flow

1. User uploads CSV file  
2. System analyzes schema  
3. Pipeline Agent generates transformation logic  
4. Data Quality Agent checks:
   - Null values  
   - Schema mismatches  
   - Data type issues  
5. BI Agent auto-generates dashboard layout  
6. Learning Agent logs feedback for improvement  

---

## 🧪 How to Test

### Option 1 – Use Sample Data

Upload:

```
/data/sample_dataset.csv
```

Prompt example:

> Create a sales summary dashboard

---

### Option 2 – Custom Data

Upload any CSV containing:
- Numeric columns  
- Date column  
- Categorical fields  

Example prompts:

- Create revenue trend report  
- Detect anomalies in monthly sales  
- Build executive dashboard  

---

## ⚠️ Known Limitations

- Requires OpenAI API access  
- Dashboard layout is auto-generated (not pixel-perfect)  
- Self-improvement stores feedback but does not retrain model  

---

## 🔮 Future Improvements

- Add Fabric pipeline auto-deployment  
- Add Power BI Service API integration  
- Add full reinforcement learning loop  
- Add multi-user access management  

---

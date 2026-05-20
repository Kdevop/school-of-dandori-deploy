# School of Dandori – AI‑Assisted Course Discovery Platform

### Executive Summary
The School of Dandori needed a modern way for learners to explore courses. All information lived in PDFs, and enrolment required knowing a specific course ID. The team delivered a prototype that extracts structured data from PDFs and presents it through a clean, searchable Streamlit interface.

### Project Context
Stakeholder interviews highlighted friction in the customer journey and operational overhead for staff. The goal of this phase was to validate whether AI‑assisted extraction and a lightweight UI could meaningfully improve discoverability while remaining simple to maintain.

### Solution Overview
The prototype includes a PDF parsing pipeline, a structured dataset, and a Streamlit interface. It is containerised for cloud deployment and designed to scale into future enrolment and instructor‑facing features.

### Architecture
- PDFs ingested from a central folder  
- Python parsing extracts structured fields  
- Data stored in a normalised CSV  
- Streamlit UI enables browsing and filtering  
- Docker container supports cloud deployment  

### Technical Components
- Python  
- Streamlit  
- Pandas  
- Custom parsing logic  
- Docker  

### Key Features
- Automated PDF extraction  
- Searchable course catalogue  
- Lightweight, cloud‑ready architecture  
- Clear foundation for future development  

---

## How to Run Locally

### 1. Clone the Repository
git clone https://github.com/Kdevop/school-of-dandori-deploy.git
cd school-of-dandori-deploy

### 2. Create a Virtual Enviroment (recomended)
python3 -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate      # Windows

### 3. Install Dependencies
pip install -r requirements.txt

### 4. Run the Streamlit App
streamlit run app.py

The app will automatically open in your browser at:
http://localhost:8501

## Run with Docker
### 1. Build the Image
docker build -t dandori-app

### 2. Run the Container
docker run -ap 8080:8080 dandori-app

The app will automatically open in your browser at:
http://localhost:8080

---

## Outputs
- Working prototype
- Extracted dataset
- Parsing scrpts and notebook
- Deployment container

---

## Future Development Opportunities
- Digital enrolement
- Instructor Dashboard
- SRM or scheduling integration
- Course demand analytics
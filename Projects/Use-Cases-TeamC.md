Suggested Tools:
https://ai.azure.com/explore/aiservices/vision/contentunderstanding?wsid=/subscriptions/1cba4dea-14a7-4215-9af9-28e9ae192225/resourcegroups/open-ai-rg/providers/Microsoft.MachineLearningServices/workspaces/project-open-ai-srv&tid=08d5cc19-84de-48f2-9dd8-344df0655d79

### Team: C - Lead Mrunali
- Individual Use cases for final selection
1. Mrunali Pusadkar - Lip and Tung Gusture and Intention Translator App - (Rank 4) (Aspirations)
2. Akshay Gulhane - Smart Grocery Inventory (Household/Shop Challenge) List Manager - (Rank 2)
3. Yogendra Bhavsar - Digitalize Electronic Health Record History from PDF Format - (Rank 1)
4. Vishal Rathod - Online Voting System (Authentication, Biometrics Identity and Bloack Chain, Internet Connectivity) - (Rank 3)

### Team C Final Use Case: Digitalize Electronic Health Record History from PDF Format
- Short Name: Digital EHR
- Web+Mobile (Progressive) Application(), Image Capture from Camera (), OCR Image Reading (), Parsing OCR data into Medical Data(), Storing into Database(), Backend API()

- Description:
1. Web application to digitalize Electronic Health Record (EHR) historically managed with paper files
2. Additionally platform will extract, organize, and manage medical history data for healthcare providers and patients.
  
- Persona:
1. Healthcare Providers: Doctors, nurses, and administrative staff looking to streamline record management.
2. Patients: Individuals who need easy access to their medical history and records.
3. Hospital Administrators: Decision-makers aiming to improve operational efficiency.
  
- Painpoint:
1. Doctors typically skimm through Patients Paper File and makes diagnosis
2. Manual extraction of patient data from PDFs is time-consuming and error-prone.
3. Difficulty in searching and accessing specific patient information.
4. Lack of interoperability between different healthcare systems.
5. Risk of data loss or duplication in physical and PDF-based records.
6. Limited data insights for analytics and reporting.

- Justification:
  1. The digitalization of health records will significantly reduce manual effort, minimize errors, and improve access to critical patient information.
  2. With growing healthcare data, an efficient, scalable, and user-friendly solution is essential to meet modern healthcare demands.
  3. Emergency: Medical History
  
- Benefits/Value:
1. Time Efficiency: Faster processing and retrieval of patient records.
2. Improved Accuracy: Automated data extraction reduces human errors.
3. Enhanced Accessibility: Easy access to records from any device.
4. Data Insights: Provides analytics for better decision-making.
5. Interoperability: Integration with existing healthcare systems and standards like HL7 or FHIR.
6. Cost Savings: Reduces administrative costs associated with paper-based systems.
  
- Current State:
1. EHRs are primarily stored in paper files.
2. Data retrieval involves manual processes.
3. Limited search and analytics capabilities.
4. Vulnerability to data loss or mismanagement.

- Proposed State:
1. A centralized, cloud-based digital EHR management system.
2. Automated extraction and indexing of data from PDFs.
3. Searchable and filterable records for healthcare providers.
4. Integration with analytics and reporting tools.
5. Secure and compliant with healthcare regulations (e.g. HIPAA, GDPR).

- Scope:
1. 

- Solution:
1. Frontend: A user-friendly React.js interface for managing records, searching, and viewing patient data.
2. Backend: Node.js and Express.js to handle API requests, user authentication, and secure data processing.
3. Database: MongoDB for storing structured patient data and metadata.
4. Data Extraction: Integration of OCR (Optical Character Recognition) tools like Tesseract.js or AWS Textract for parsing PDFs.
5. Cloud Hosting: Deploy on cloud platforms like AWS or Azure for scalability and security.
6. Security: Implement role-based access control (RBAC), encryption, and compliance standards.
7. Analytics: Provide dashboards for data insights using tools like Chart.js or D3.js.
9. AI Data Extraction: 

- Technologies:
1. Using the MERN (MongoDB, Express.js, React.js, Node.js) stack
2. Frontend: React.js, Tailwind CSS/Material-UI for design.
3. Backend: Node.js, Express.js.
4. Database: MongoDB.
5. OCR Tools: Tesseract.js, AWS Textract, or Google Cloud Vision API.
6. Hosting: AWS, Azure, or Heroku.
7. Authentication: JWT (JSON Web Token) or OAuth2.
8. Analytics: Chart.js, D3.js, or Power BI integration.

- Use Case Methodology: SIPOC
1. Supplier: Patient/Assistance (Mobile App)
2. Input: (Scan Record) --> PDF --> Upload
3. Process: (Web Application) --> Processing 
4. Output: Patient Account History in PDF and Text
5. Customer: Physician/Patient/Associate(Medical History)
    

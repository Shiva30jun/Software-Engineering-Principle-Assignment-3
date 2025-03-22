# **AI Training Data - Actionable Requirements**

## **Project Overview**

Our client, an AI developer, uses web scraping to collect training data for their AI models. They've identified four critical areas to improve data quality and model performance

## **UR-01: Categorized Training Questions**

**Title:**  
_As an AI developer, I want training questions to be organized into categories so that I can separate them from their answers and enhance my self-evaluation process._

**GitHub Issue:** #1

### **Purpose**

After talking to the client, the client has reported that they want to organize questions into categories so developers can easily focus on specific areas and track their understanding.

So, from this, we have decided to implement a categorization feature with a dropdown interface for tagging questions and storing them by topic.

### **Implementation Strategy**

We will build a dropdown menu to allow users to tag training questions with predefined categories. When the user submits a question, the category will be saved alongside the entry in the database. This will help sort and filter questions during training.

- Create UI with dropdown selector  
- Accept question and selected category from user  
- Save both question and category to database  
- Retrieve and display questions by category  

### **Sub-Issues**

**Sub-Issue 1:**  
A well-organized Q&A format improves learning and prevents unintentional answer hints.  
**Validation:** Conduct usability testing with developers to confirm improved focus and usability.

**Sub-Issue 2: Implement Question Categorization UI**  
**Goal:** Allow users to assign categories to questions.  
**Approach:** Integrate dropdown and backend saving logic.  
**Tasks:**
- Create dropdown for category selection.
- Store selected category with each question entry.
- Connect UI with backend API.
- Validate selected category before saving.
- Load category options dynamically from database or config.

---

## **UR-02: Balanced Training Data**

**Title:**  
_As an AI developer, I want balanced training data so that AI models do not develop biases and provide more reliable results._

**GitHub Issue:** #2

### **Purpose**

After talking to the client, the client has reported that their AI models were unintentionally biased due to unbalanced datasets.

So from this, we have decided to implement bias detection scripts that analyse frequency distributions and flag overrepresented data.

### **Implementation Strategy**

We will write scripts to measure the distribution of values across dataset features. These will be checked against thresholds to detect imbalances. Any overrepresented categories will be flagged, visualized, and documented in reports.

- Identify key data features to analyse  
- Calculate value frequencies  
- Flag categories above a threshold  
- Output flagged results to reports 

### **Sub-Issues**

**Sub-Issue 1:**  
We assume that removing bias from training data improves model performance and fairness.  
**Validation:** Compare model performance before and after dataset balancing.

**Sub-Issue 2: Implement Bias Detection Algorithm**  
**Goal:** Detect and report bias in the dataset.  
**Approach:** Use rule-based frequency checks.  
**Tasks:**
- Identify common indicators of dataset bias.
- Write frequency analysis scripts.
- Set thresholds for category overrepresentation.
- Log flagged data with bias scores.
- Export results in CSV format.
- Visualize bias using bar/pie charts.
- Save visualizations in a centralized dashboard folder.

**Sub-Issue 3: Workflow for Maintaining Balanced Data**  
**Goal:** Maintain data balance continuously.  
**Approach:** Automate threshold checks and alerts.  
**Tasks:**
- Define balance thresholds for each feature.
- Build automated alerts for imbalance detection.
- Schedule weekly checks to flag anomalies.

---

## **UR-03: Training Data Quality Monitoring**

**Title:**  
_As an AI developer, I want an automated system to monitor training data quality so that dataset balance is maintained._

**GitHub Issue:** #3

### **Purpose**

After talking to the client, the client has reported that maintaining consistent quality across their large training datasets has become challenging.

So from this, we have decided to implement automated indicators, alerts, and reporting tools to monitor data quality continuously.

### **Implementation Strategy**

We will define key quality indicators and monitor them automatically. Alerts will be triggered when values deviate from expected norms, and weekly reports will be shared with the team.

- Set thresholds for data balance  
- Monitor new data in real time  
- Trigger alerts for outliers  
- Email weekly quality reports  


### **Sub-Issues**

**Sub-Issue 1:**  
We assume that continuous monitoring helps ensure long-term dataset integrity.  
**Validation:** Compare weekly data snapshots to detect shifts or imbalance trends.

**Sub-Issue 2: Develop Alerts for Quality Issues**  
**Goal:** Notify developers of data inconsistencies in real time.  
**Approach:** Monitor and benchmark live data streams.  
**Tasks:**
- Monitor input sources in real time.
- Compare with pre-defined benchmarks.
- Trigger email/SMS alerts on deviations.

**Sub-Issue 3: Generate Data Quality Reports**  
**Goal:** Provide developers with regular quality updates.  
**Approach:** Use automated scripts to pull, format, and share reports.  
**Tasks:**
- Pull daily/weekly data health metrics.
- Format and email reports to stakeholders.
- Archive reports in a structured folder for auditing.

---

## **UR-04: Scalable Data Handling**

**Title:**  
_As an AI developer, I want a system that can efficiently process large datasets so that AI models can be trained without performance issues._

**GitHub Issue:** #4





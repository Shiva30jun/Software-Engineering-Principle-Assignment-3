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



# 🧠 Student Feedback Topic Modeling — AI-Driven Courses Analysis

## 🎯 Project Overview
A Delhi-based online learning startup aims to analyze large volumes of student feedback for its newly launched AI-driven courses. Due to the absence of real-world feedback data, a synthetic dataset was generated to simulate realistic student opinions covering aspects like course content, instructor quality, engagement, and platform usability.

***

## 🛠️ Workflow to Solve the Problem
**Step 1: Data Understanding**  
- Using dataset that contains synthetic text feedback for AI courses.  
- Each record represents one student's opinion.

**Step 2: Data Preprocessing**  
- Text normalized to lowercase, nulls and punctuation removed.  
- Stopwords filtered out; tokenized for analysis.

**Step 3: TF-IDF Vectorization**  
- Numerical representation of text using `TfidfVectorizer`.  
- Parameters: `stop_words='english'`, `max_df=0.9`, `min_df=2`, `max_features=1000`.

**Step 4: Topic Modeling (NMF)**  
- Non-negative Matrix Factorization to extract 5 latent topics.  
- Identified topic-defining keywords representing key feedback themes.

**Step 5: Topic Assignment**  
- Each feedback assigned to dominant topic based on highest NMF weight.  
- Output saved in `feedback_with_topics.csv`.

**Step 6: Visualization**  
- Bar charts created with Matplotlib and Seaborn highlighting topic prevalence.

***
## Topic Modelling Snapshot 

| **Topic** | **Top Keywords**                                   | **Possible Interpretation**             |
| :-------: | :------------------------------------------------- | :-------------------------------------- |
|   **1**   | instructor, explanation, engaging, teaching, style | Instructor quality and teaching clarity |
|   **2**   | assignments, practical, real, projects, learning   | Hands-on learning & project experience  |
|   **3**   | platform, bugs, interface, speed, login            | Platform usability and technical issues |
|   **4**   | ai, models, examples, concepts, accuracy           | Course depth and technical content      |
|   **5**   | feedback, improvement, updates, doubt, response    | Student support and responsiveness      |

***

## 🔎 Interpretation — Expanded Insights & Recommendations

### Instructor Quality 
Students commend engaging instructors but highlight the need for clearer explanations to strengthen understanding.  

**Recommendation:**  
- Regular faculty training sessions emphasizing clarity.  
- Promote interactive teaching and student engagement workshops.

### Practical Learning 
Practical assignments and real-life projects are highly valued, enhancing knowledge retention.  

**Recommendation:**  
- Include capstone projects and industry case studies.  
- Deploy AI labs and project-based learning modules.

### Platform Usability
Feedback frequently mentions bugs and slow or confusing interfaces impacting learning engagement.  

**Recommendation:**  
- Prioritize UI/UX improvements and mobile responsiveness.  
- Develop a dedicated bug reporting and rapid fix system.

### Course Depth
Interest in deeper AI concepts such as model accuracy and concepts indicates room for advanced modules.  

**Recommendation:**  
- Provide modular content with advanced AI tracks.  
- Increase examples and hands-on exercises covering key AI algorithms.

### Student Support
Requests for fast query resolution and better feedback highlight support improvement areas.  

**Recommendation:**  
- Implement chatbot and mentor support for real-time queries.  
- Establish regular feedback collection and response analysis.

***

## 🛠️ Tools & Libraries- Python 3.13  
- Pandas  
- Scikit-learn  
- Matplotlib / Seaborn  

***

## ⚠️ Disclaimer
This work is for educational purposes only and does not constitute professional advice. Interpret results considering the synthetic nature of feedback data.

***


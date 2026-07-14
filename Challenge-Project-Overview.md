---

> ## Challenge Advisor: Update & Finalize Your Project Overview
>
> > 💡 **These grey text instructions are just for you, the team's Challenge Advisor; please delete them once you have completed the steps below.**
>
> We've pre-populated this Challenge Project Overview page — which is what will be shared with your Break Through Tech student team in August — using the details from your submission form. You should have received an email inviting you to join this repo as a Collaborator, enabling you to add files and make edits.
> 
> In order for your project to be finalized and assigned to a team, please:
> 1. **Review all sections below** and update or expand any content as needed, making sure to address the SME Feedback in the section immediately below. Look for square brackets to find the places below that require additional inputs from you (e.g., "About [Company / Org Name]").
> 2. **Add your dataset** to the [data folder](data) in this repo.
> 3. **Close the Issue assigned to you in this repo** to let us know that you have made your edits and the overview page is ready for final review. You can do this by going to the _Issues_ tab in the top left section of the menu above, add a comment that says "CA review complete", and click the button to Close the Issue. 
>
> If you're unfamiliar with how to edit a page like this in GitHub, check out [this tutorial](https://ubc-lib-geo.github.io/gis-workshop-waml-template/content/handson/edit-readme.html) for a quick overview (start with step 2 and only edit this page), and [this guide](https://ubc-lib-geo.github.io/gis-workshop-waml-template/content/markdown.html) on how to use Markdown to compose text.
>
>
> ❌ Remember that this is a public repo. Do NOT include: Proprietary data, PII, API keys, credentials, or anything confidential.

---

## 📋 BTT Internal Evaluation Notes
*(This section is for BTT staff and CAs only — remove before sharing with students)*

### Technical Vetting
| Check | Status | Notes |
| :--- | :--- | :--- |
| Python Compatibility | 🟢 | Project utilizes standard NLP ecosystem (HuggingFace Transformers, PyTorch, Scikit-learn), which is fully compatible with Google Colab. |
| Data Readiness | 🟢 | Bitext and CLINC150 are well-documented, standard benchmark datasets for intent classification. |
| Resource Check | 🟡 | While Free-tier Colab is requested, fine-tuning Phi-2 or DistilBERT can hit VRAM limits. Reliance on external LLM APIs for teacher labeling incurs costs and potential quota issues. |

### Internal Scores
- **Student Fit Score:** 7/10
- **Technical Depth Score:** 8/10
- **Overall Recommendation:** REVISE

### Advisor Feedback Draft
This project offers a high-impact exploration of model distillation, which is a vital skill in modern Enterprise AI. To succeed within the 12-week BTT timeline, I recommend two adjustments: 1) Reduce the synthetic dataset size to 5k-10k high-quality samples to stay within budget/time, and 2) Use a local open-source teacher model (e.g., Llama-3-8B via Ollama or HuggingFace) for label generation to remove dependency on proprietary API keys. 

---

# Domain-Specific Theme Labeling via SLM Distillation

**Company / Org:** Automation Anywhere  
**Challenge Advisor:** Archan Dutta, archanduttads@gmail.com  
**Program:** Break Through Tech AI Studio - Fall 2026  

---

## 🏢 About Automation Anywhere
Automation Anywhere is a global leader in Intelligent Automation, specializing in Robotic Process Automation (RPA) and AI-driven business solutions. The company empowers organizations to scale their operations through digital transformation, focusing on deploying intelligent software bots to handle complex business processes efficiently.

---

## 🎯 The Challenge
### Project Summary
This project explores knowledge distillation by using high-performing Large Language Models (LLMs) to label support datasets and train compact Small Language Models (SLMs). By optimizing models for IT, HR, and CX domains, the team will demonstrate a path to achieving enterprise-grade classification accuracy while significantly reducing computational costs and inference latency.

### Success Criteria
SLM achieves ≥ 90% of LLM accuracy on theme classification (macro F1). ≥ 10x reduction in cost-per-1,000-labels vs. GPT-4 API pricing. ≥ 5x reduction in inference latency (measured on Colab T4). Demo: real-time side-by-side output comparing LLM vs. SLM on live ticket input.

### Project Milestones
Use these milestones to guide your work. Your team will create a GitHub Projects board to track tasks within each milestone.
| Month | Milestone | Key Activities |
|-------|-----------|----------------|
| **September** | Data Exploration & Preprocessing | Acquire Bitext and CLINC150 datasets, perform exploratory data analysis, and sanitize inputs to prepare for LLM labeling. |
| **October** | Feature Engineering & Baseline Modeling | Design and iterate on LLM prompts to generate 20k-30k silver-labeled examples and establish baseline performance metrics. |
| **November** | Model Optimization & Evaluation | Fine-tune DistilBERT and Phi-2 models, benchmarking performance against the teacher model to ensure target accuracy. |
| **December** | Insights, Deliverables & Presentation | Develop a Streamlit demo for real-time visualization and compile the final report detailing ROI, cost savings, and technical findings. |

> **Note for the team:** Please create a GitHub Projects board in this repository to break these milestones into weekly tasks. Go to the **Projects** tab → **New project** → Choose **Board** → Add columns for each month.

---

## 📊 Dataset
**Name and Source:** Bitext and CLINC150 (Public Open-Source NLP Benchmarks)  
**Format:** JSON / CSV  
**Size:** 1gb to 5gb  
**Location:** HuggingFace Datasets Hub  

### Key Details
- IT/HR/CX Support Datasets
- Requires strict mapping of raw support tickets to standardized intent categories, ensuring label quality through prompt engineering and data validation checks.

---

## 🛠️ Suggested Approach
**ML Problem Type:** NLP & RAG / Classification  
**Recommended Libraries:** HuggingFace Transformers, PyTorch, Scikit-learn, Streamlit  
**Evaluation Metrics:** Macro F1 Score, Inference Latency (ms), Cost per 1,000 requests, VRAM usage.

---

## 📚 Resources to Get Started
The following resources will help your team understand the problem space and potential technical approaches for this project:
**Background Reading:**
- HuggingFace Guide to Knowledge Distillation
**Technical Tutorials:**
- Fine-tuning BERT for Sequence Classification
**Code Examples:**
- HuggingFace Transformers Documentation for Distillation

---

## 🤝 How We'll Work Together
**Check-ins:** During our biweekly 60-min AI Studio Lab Section meeting block (2nd and 4th week of every month)  
**Communication:** Slack / Email  
**Response time:** 24-48 business hours  
**Recommended Tools:**
- **Coding:** Google Colab Free Tier  
- **Collaboration:** GitHub, Notion  
- **Virtual Meetings:** Zoom, Google Meet  

---

## 🚀 Getting Started
1. **Review this overview document** and note any questions for our first meeting.
2. **Begin reviewing the dataset** using the link provided in the Dataset section.
3. **Read the GitHub Projects documentation** [here](https://docs.github.com/en/issues/planning-and-tracking-with-projects/learning-about-projects/about-projects).

I'm excited to work with you!

---

## ❓ Questions?
Please bring any questions to our first meeting during the week of August 24th (Break Through Tech's Bridge to Studio - Session B).

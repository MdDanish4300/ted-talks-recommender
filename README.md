# 🎯 Personalized TED Talks Recommendation System Using Machine Learning

A machine learning-based recommendation system developed as part of the **Infosys Springboard Virtual Internship 7.0**.

The project aims to help users discover relevant TED Talks by analyzing talk transcripts, tags, metadata, and user preferences where suitable interaction data is available.

## 📌 Project Overview

TED Talks cover a wide range of subjects, including technology, science, education, psychology, business, and personal development. With thousands of talks available, discovering content relevant to individual interests can be challenging.

This project aims to build a machine learning-based recommendation system that suggests relevant TED Talks by analyzing their content and, where data permits, user preferences and behavior.

The initial approach will focus on **content-based filtering** using text preprocessing, feature engineering, TF-IDF vectorization, and cosine similarity. Collaborative filtering and hybrid approaches will be investigated if suitable user–item interaction data is available.

The recommendation engine will ultimately be integrated into an interactive web application using Streamlit.

## 🎯 Project Objectives

* Collect and understand TED Talks metadata and transcripts.
* Perform exploratory data analysis (EDA) and data preprocessing.
* Identify and handle missing values, duplicates, and inconsistencies.
* Clean and prepare textual and categorical features.
* Apply feature engineering and text vectorization techniques.
* Develop a suitable recommendation engine.
* Evaluate recommendation quality using appropriate metrics.
* Deploy an interactive recommendation application using Streamlit.
* Document the implementation, evaluation, and deployment process.

## ✨ Planned Features

* **TED Talks Exploration:** Explore talks using available metadata, tags, descriptions, and speaker information.
* **Content-Based Recommendations:** Recommend talks based on similarities in their textual content and metadata.
* **Personalized Discovery:** Help users discover talks based on selected interests, tags, or a previously liked talk.
* **Recommendation Evaluation:** Evaluate recommendation quality using appropriate metrics.
* **Interactive Web Interface:** Present recommendations through a user-friendly Streamlit application.
* **Explainable Recommendations:** Where feasible, explain why a particular talk was recommended.
* **Project Documentation:** Document the methodology, implementation decisions, evaluation results, and deployment process.

These are planned capabilities. Features will be marked as implemented only after development and testing.

## 🛠️ Technology Stack

| Technology         | Purpose                                                                    |
| ------------------ | -------------------------------------------------------------------------- |
| Python             | Core programming language                                                  |
| Pandas             | Data manipulation and analysis                                             |
| NumPy              | Numerical operations                                                       |
| Matplotlib         | Data visualization                                                         |
| Seaborn            | Statistical visualization                                                  |
| Scikit-learn       | Text vectorization, preprocessing, similarity calculations, and evaluation |
| Jupyter Notebook   | Exploratory data analysis and experimentation                              |
| Streamlit          | Interactive web application                                                |
| Git                | Version control                                                            |
| GitHub             | Source code hosting and project documentation                              |
| Visual Studio Code | Development environment                                                    |

The final dependencies will be documented in `requirements.txt` as implementation progresses.

## 🧠 Recommendation Methodology

The final recommendation strategy will be selected based on data availability, implementation feasibility, and evaluation results.

### 1. Content-Based Filtering

Content-based filtering will identify TED Talks similar to a selected talk or a user's interests by analyzing available talk information.

Potential techniques include:

* Text cleaning and preprocessing
* TF-IDF vectorization
* Cosine similarity
* Feature engineering using tags and metadata
* Text embeddings, if appropriate

The initial implementation will focus on TF-IDF and cosine similarity.

### 2. Collaborative Filtering

Collaborative filtering will be investigated if suitable user–item interaction data, such as ratings or watch history, is available.

The project will assess the availability and quality of interaction data before deciding whether collaborative filtering can be implemented meaningfully.

### 3. Hybrid Recommendations

A hybrid approach may combine content-based and collaborative signals if the available data supports both.

The final recommendation strategy will be selected after implementation and evaluation.

## 📂 Project Structure

```text
ted-talks-recommender/
├── data/
│   ├── ted_main.csv
│   └── transcripts.csv
├── notebooks/
├── src/
├── .gitignore
├── README.md
└── requirements.txt
```

**Note:**

* The `data/` directory contains datasets stored locally on the development machine.
* The CSV datasets and Python virtual environment are excluded from Git version control.
* The `notebooks/` directory will contain EDA and experimentation notebooks.
* The `src/` directory will contain reusable project implementation code.
* `requirements.txt` will document the project's dependencies as they are finalized.

The project structure will evolve as development progresses.

## 📊 Dataset

The project currently uses two CSV files obtained through Kaggle.

### 1. `ted_main.csv`

Contains TED Talks metadata, including available information such as:

* Talk titles
* Speaker names and occupations
* Descriptions
* Tags
* Other talk-related metadata

### 2. `transcripts.csv`

Contains transcript text associated with TED Talks.

The metadata and transcript datasets will be examined to understand their structure, data quality, and relationships.

### Initial Data Exploration

Initial exploration has included:

* Loading the datasets for analysis.
* Examining frequently occurring TED Talk tags.
* Checking missing values in selected metadata columns.

The next steps include comprehensive data-quality checks, further EDA, and preprocessing.

### Dataset Licensing

The datasets are stored locally and are excluded from the Git repository.

Their original sources, attribution requirements, and redistribution conditions must be verified before distributing the files.

Dataset source attribution and download instructions will be documented after verification.

## 🚀 Getting Started

### Prerequisites

* Python 3.x
* Git
* Visual Studio Code

### 1. Clone the Repository

```bash
git clone https://github.com/MdDanish4300/ted-talks-recommender.git
```

### 2. Navigate to the Project Directory

```bash
cd ted-talks-recommender
```

### 3. Create a Virtual Environment

On Windows PowerShell:

```powershell
python -m venv venv
```

### 4. Activate the Virtual Environment

```powershell
.\venv\Scripts\Activate.ps1
```

### 5. Install Dependencies

Once `requirements.txt` has been created and populated, install the dependencies using:

```powershell
python -m pip install -r requirements.txt
```

### 6. Prepare the Dataset

Obtain the required datasets from the verified source and place them in the local `data/` directory.

Ensure that the filenames match those expected by the project code.

**Important:** The datasets are not downloaded automatically when cloning the repository. They are excluded from version control and must be obtained separately.

## 🗺️ Implementation Roadmap

The project follows the four milestones and seven modules specified in the official internship project document.

### Milestone 1 — Data Collection and Preprocessing

**Timeline: Weeks 1–2**

**Module 1: Data Collection**

* [x] Obtain the initial TED Talks metadata and transcript datasets.
* [ ] Verify dataset sources and licensing.
* [ ] Document dataset sources and attribution.
* [ ] Assess dataset coverage and available fields.

**Module 2: Data Exploration and Data Preprocessing**

* [x] Load the datasets for initial analysis.
* [x] Explore frequently occurring TED Talk tags.
* [x] Check missing values in selected metadata columns.
* [ ] Inspect dataset completeness, columns, and data types.
* [ ] Investigate duplicate records and inconsistencies.
* [ ] Analyze talk lengths and tag distributions.
* [ ] Investigate missing transcripts and tags.
* [ ] Clean text by applying suitable normalization and preprocessing.
* [ ] Handle missing values appropriately.
* [ ] Encode relevant categorical features where necessary.
* [ ] Investigate user–item interaction data if available.
* [ ] Generate EDA visualizations and summary statistics.
* [ ] Prepare the cleaned dataset for feature extraction and modeling.

**Expected Deliverables**

* Cleaned and preprocessed dataset.
* Data-quality summary and statistics.
* Visualizations of talk lengths and tag frequencies.
* Documented preprocessing workflow.

### Milestone 2 — Feature Engineering and Recommendation Engine

**Timeline: Weeks 3–4**

**Module 3: Feature Engineering and Vectorization**

* [ ] Select and document suitable text preprocessing techniques.
* [ ] Apply TF-IDF or an appropriate embedding technique.
* [ ] Generate numerical representations of talk content.
* [ ] Engineer relevant textual and metadata features.
* [ ] Analyze and visualize similarity scores.
* [ ] Save the selected vectorizer or embedding model.
* [ ] Investigate a user–item interaction matrix if suitable data is available.
* [ ] Document vectorization choices and parameter settings.

**Module 4: Develop Recommendation Engine**

* [ ] Implement the initial content-based recommendation approach.
* [ ] Calculate similarity between TED Talks.
* [ ] Develop a function that returns the top-N similar talks.
* [ ] Test recommendations using sample talks.
* [ ] Investigate collaborative filtering if interaction data is available.
* [ ] Explore a hybrid approach if feasible.
* [ ] Define a suitable training and testing strategy for offline evaluation.
* [ ] Save reusable models and artifacts.
* [ ] Document model design and implementation decisions.

**Expected Deliverables**

* TF-IDF or embedding representations.
* Saved vectorizer or embedding artifacts.
* Similarity scores or matrices.
* Working recommendation engine.
* Notebooks or scripts demonstrating the implementation.
* Documented recommendation methodology.

### Milestone 3 — Evaluation Metrics

**Timeline: Weeks 5–6**

**Module 5: Evaluation Metrics**

* [ ] Define an appropriate evaluation strategy.
* [ ] Evaluate recommendation quality using suitable metrics.
* [ ] Investigate Precision, Recall, NDCG, and Mean Average Precision where applicable.
* [ ] Compare recommendation approaches where feasible.
* [ ] Analyze the trade-offs between content-based and collaborative filtering.
* [ ] Visualize evaluation results.
* [ ] Select the final model based on performance and interpretability.
* [ ] Document the rationale for model selection.

**Expected Deliverables**

* Evaluation reports and plots.
* Model comparison tables.
* Documented evaluation methodology.
* Justification for the selected recommendation approach.

### Milestone 4 — Deployment and Documentation

**Timeline: Weeks 7–8**

**Module 6: Deployment via Streamlit**

* [ ] Design an interactive Streamlit application.
* [ ] Integrate the selected recommendation engine.
* [ ] Provide user input options, such as selecting a talk or choosing tags.
* [ ] Display top-N recommendations with available talk details.
* [ ] Include content-based explanations where feasible.
* [ ] Test the recommendation workflow and application.
* [ ] Document local execution and deployment.

**Module 7: Presentation and Documentation**

* [ ] Document all project modules and implementation decisions.
* [ ] Include EDA visualizations and evaluation results.
* [ ] Capture screenshots of the application.
* [ ] Prepare presentation slides summarizing the project.
* [ ] Document installation and deployment.
* [ ] Review the repository for reproducibility and clarity.
* [ ] Complete the final code submission.

**Expected Deliverables**

* Functional Streamlit application.
* Screenshots demonstrating recommendations.
* Installation and deployment documentation.
* Final project report and presentation slides.
* Reproducible code in the GitHub repository.

## 📈 Current Progress

### Completed

* [x] Created the local project directory.
* [x] Created the Python virtual environment.
* [x] Installed and verified the initial Python libraries.
* [x] Obtained the TED Talks metadata and transcript datasets.
* [x] Created the `data/`, `notebooks/`, and `src/` directories.
* [x] Loaded the datasets for initial exploration.
* [x] Identified frequently occurring TED Talk tags.
* [x] Checked missing values in selected metadata columns.
* [x] Initialized the local Git repository.
* [x] Configured `.gitignore` to exclude datasets and the virtual environment.
* [x] Created the initial project README.
* [x] Connected the local repository to GitHub.
* [x] Created the initial Git commit and pushed it to the `main` branch.
* [x] Submitted the GitHub repository details for internship tracking.

### In Progress

* [ ] Continue exploratory data analysis.
* [ ] Inspect dataset columns, data types, and distributions.
* [ ] Investigate missing values, duplicates, and data inconsistencies.
* [ ] Examine the relationship between talk metadata and transcripts.
* [ ] Verify dataset licensing and document source attribution.
* [ ] Clean and preprocess the datasets.
* [ ] Prepare the data for feature engineering.

### Upcoming

* [ ] Apply TF-IDF vectorization.
* [ ] Calculate cosine similarity between TED Talks.
* [ ] Implement and test the content-based recommendation engine.
* [ ] Investigate collaborative filtering if suitable interaction data is available.
* [ ] Evaluate recommendation quality.
* [ ] Develop the Streamlit application.
* [ ] Complete project documentation and presentation.

Progress will be updated as tasks are completed and verified.

## 🎓 Internship Information

**Program:** Infosys Springboard Virtual Internship 7.0

**Project:** Personalized TED Talks Recommendation System Using Machine Learning

**Duration:** Eight-week virtual internship

## 👨‍💻 Author

**Md Danish**

BCA Student | Aspiring Software Developer | Machine Learning Enthusiast

GitHub: [@MdDanish4300](https://github.com/MdDanish4300)

**Repository:** [ted-talks-recommender](https://github.com/MdDanish4300/ted-talks-recommender)

---

*This project is being developed for educational purposes as part of the Infosys Springboard Virtual Internship 7.0.*

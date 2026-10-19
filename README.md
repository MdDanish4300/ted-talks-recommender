# 🎯 Personalized TED Talks Recommendation System Using Machine Learning

A machine learning-based recommendation system being developed as part of the **Infosys Springboard Virtual Internship 7.0**.

The project aims to help users discover relevant TED Talks based on their interests by analyzing talk metadata, tags, descriptions, and transcript content.

## 📌 Project Overview

TED Talks cover a wide range of subjects, including technology, science, education, psychology, business, and personal development. With thousands of talks available, finding content relevant to individual interests can be challenging.

This project aims to develop a recommendation system that analyzes TED Talk content and recommends relevant talks based on content similarity and user interests.

The project will explore content-based filtering using text processing, feature engineering, and similarity calculations. Collaborative or hybrid approaches may also be investigated if suitable user–item interaction data is available.

The final recommendation engine will be integrated into an interactive web application using Streamlit.

## 🎯 Project Objectives

- Collect and understand TED Talks metadata and transcripts.
- Perform exploratory data analysis (EDA).
- Identify missing values, duplicates, and data inconsistencies.
- Clean and preprocess textual and categorical features.
- Apply feature engineering and text vectorization techniques.
- Develop a suitable recommendation engine.
- Evaluate recommendation quality using appropriate metrics.
- Build an interactive Streamlit application.
- Document the implementation, evaluation, and deployment process.

## ✨ Planned Features

- **TED Talks Exploration:** Explore talks using available metadata, topics, tags, and speaker information.
- **Content-Based Recommendations:** Recommend talks based on similarities in their textual content and metadata.
- **Personalized Discovery:** Help users discover talks relevant to their interests.
- **Recommendation Evaluation:** Evaluate the recommendation engine using suitable metrics.
- **Interactive Web Interface:** Present recommendations through a user-friendly Streamlit application.
- **Explainable Recommendations:** Where feasible, explain why a particular talk was recommended.
- **Documentation:** Provide implementation details, evaluation results, and setup instructions.

These are planned capabilities. Features will be marked as implemented only after development and testing.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Preprocessing, vectorization, similarity calculations, and evaluation |
| Jupyter Notebook | Exploratory data analysis and experimentation |
| Streamlit | Interactive web application |
| Git | Version control |
| GitHub | Source code hosting and project documentation |
| Visual Studio Code | Development environment |

The final dependencies will be documented in `requirements.txt` as implementation progresses.

## 🧠 Recommendation Approach

The final recommendation strategy will be selected based on data availability, implementation feasibility, and evaluation results.

### 1. Content-Based Filtering

Content-based filtering will use information about TED Talks to identify talks similar to a user's interests or a selected talk.

Potential techniques include:

- Text preprocessing and normalization
- TF-IDF vectorization
- Cosine similarity
- Metadata-based feature engineering
- Text embeddings, if appropriate

### 2. Collaborative Filtering

Collaborative filtering may be investigated if suitable user–item interaction data, such as ratings or viewing history, is available.

The availability and quality of such data will determine whether this approach can be implemented meaningfully.

### 3. Hybrid Recommendations

A hybrid approach may combine content-based and collaborative signals if the available data supports both.

The project will prioritize a practical recommendation approach that can be implemented and evaluated reliably.

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
- The `data/` directory contains the datasets stored locally on the development machine.
- The CSV datasets and Python virtual environment are excluded from Git version control.
- The `notebooks/` and `src/` directories will contain analysis notebooks and implementation code as development progresses.
- `requirements.txt` will be created and maintained as project dependencies are finalized.

The structure will evolve as the project develops.

## 📊 Dataset

The project currently uses two CSV files obtained through Kaggle.

### 1. `ted_main.csv`

Contains TED Talks metadata, including available information such as:

- Talk titles
- Speakers and speaker occupations
- Descriptions
- Tags
- Other talk-related metadata

### 2. `transcripts.csv`

Contains transcript text associated with TED Talks.

The metadata and transcript datasets will be examined to understand their structure and determine how records correspond to one another.

### Data Collection and Initial Analysis

The datasets have been obtained and loaded for initial exploration.

Initial analysis has included:
- Examining frequently occurring TED Talk tags.
- Checking missing values in selected metadata columns.
- Beginning to understand the available data fields.

The next steps include further exploratory data analysis, data-quality checks, and preprocessing.

### Dataset Licensing

The datasets are stored locally and are excluded from the Git repository.

Their original sources, attribution requirements, and redistribution conditions must be verified before distributing the files.

Dataset download instructions and source attribution will be documented after verification.

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- Git
- Visual Studio Code

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

The project follows the four milestones specified in the internship project document.

### Milestone 1 — Data Collection and Exploration

- [x] Obtain the initial TED Talks metadata and transcript datasets.
- [x] Load the datasets for initial analysis.
- [x] Explore frequently occurring TED Talk tags.
- [x] Check missing values in selected metadata columns.
- [ ] Verify dataset sources and licensing.
- [ ] Complete dataset structure and data-type inspection.
- [ ] Investigate duplicate records and data inconsistencies.
- [ ] Examine the relationship between metadata and transcripts.
- [ ] Complete exploratory data analysis.
- [ ] Clean and preprocess the relevant data.
- [ ] Generate useful visualizations and summary statistics.

### Milestone 2 — Feature Engineering and Recommendation Engine

- [ ] Select suitable text preprocessing techniques.
- [ ] Prepare and combine relevant textual and metadata features.
- [ ] Select and implement text vectorization techniques.
- [ ] Generate numerical representations of talk content.
- [ ] Calculate content similarity scores.
- [ ] Implement the content-based recommendation engine.
- [ ] Investigate collaborative filtering if suitable interaction data is available.
- [ ] Compare feasible recommendation strategies.
- [ ] Document model design and implementation decisions.

### Milestone 3 — Evaluation

- [ ] Define an appropriate evaluation strategy.
- [ ] Evaluate recommendation quality using suitable metrics.
- [ ] Investigate Precision, Recall, NDCG, and Mean Average Precision where applicable.
- [ ] Compare recommendation approaches where feasible.
- [ ] Document evaluation results and model selection.

### Milestone 4 — Deployment and Documentation

- [ ] Develop the Streamlit application.
- [ ] Integrate the selected recommendation engine.
- [ ] Display relevant TED Talk recommendations.
- [ ] Test the application and recommendation workflow.
- [ ] Document installation and deployment.
- [ ] Prepare application screenshots and presentation slides.
- [ ] Complete the final project documentation.

## 📈 Current Progress

### Completed

- [x] Created the local project directory.
- [x] Created the Python virtual environment.
- [x] Installed and verified the initial Python libraries.
- [x] Obtained the TED Talks metadata and transcript datasets.
- [x] Created the `data/`, `notebooks/`, and `src/` directories.
- [x] Loaded the datasets for initial exploration.
- [x] Identified frequently occurring TED Talk tags.
- [x] Checked missing values in selected metadata columns.
- [x] Initialized the local Git repository.
- [x] Created and configured `.gitignore`.
- [x] Created the initial project README.
- [x] Connected the local repository to GitHub.
- [x] Created the initial commit and pushed it to the `main` branch.

### In Progress

- [ ] Continue exploratory data analysis.
- [ ] Inspect dataset columns, data types, and distributions.
- [ ] Investigate missing values and duplicate records.
- [ ] Examine the relationship between talk metadata and transcripts.
- [ ] Verify dataset licensing and document source attribution.
- [ ] Clean and preprocess the data.

### Upcoming

- [ ] Prepare features for the recommendation engine.
- [ ] Implement and evaluate the recommendation approach.
- [ ] Develop the Streamlit application.
- [ ] Complete testing and project documentation.

Progress will be updated as tasks are completed and verified.

## 🎓 Internship Information

**Program:** Infosys Springboard Virtual Internship 7.0

**Project:** Personalized TED Talks Recommendation System Using Machine Learning

**Duration:** Eight-week virtual internship

## 👨‍💻 Author

**Md Danish**

BCA Student | Aspiring Software Developer | Machine Learning Enthusiast

GitHub: [@MdDanish4300](https://github.com/MdDanish4300)

---

*This project is being developed for educational purposes as part of the Infosys Springboard Virtual Internship 7.0.*

# 🎯 Personalized TED Talks Recommendation System Using Machine Learning

A machine learning-based recommendation system developed as part of the **Infosys Springboard Virtual Internship 7.0**.

The project aims to help users discover relevant TED Talks based on their interests by analyzing talk metadata, tags, and transcript content.

## 📌 Project Overview

TED Talks cover a wide range of subjects, including technology, science, education, psychology, business, and personal development. With thousands of talks available, discovering content relevant to individual interests can be challenging.

This project aims to develop a personalized recommendation system that analyzes TED Talk content and, where suitable interaction data is available, user preferences to generate relevant recommendations.

The system will explore content-based filtering and, where the available data supports it, collaborative or hybrid recommendation techniques. The final recommendation engine will be integrated into an interactive web application using Streamlit.

## 🎯 Project Objectives

- Collect and understand TED Talks metadata and transcripts.
- Perform exploratory data analysis (EDA) and data preprocessing.
- Clean and prepare textual and categorical features.
- Apply feature engineering and text vectorization techniques.
- Develop a suitable recommendation engine.
- Evaluate recommendation quality using appropriate evaluation metrics.
- Build an interactive Streamlit application.
- Document the implementation, evaluation, and deployment process.

## ✨ Planned Features

- **TED Talks Exploration:** Explore talks using available metadata, topics, tags, and speaker information.
- **Content-Based Recommendations:** Recommend talks based on similarities in their textual content and metadata.
- **Personalized Discovery:** Support interest-based recommendations through suitable user inputs.
- **Recommendation Evaluation:** Evaluate the recommendation engine using appropriate metrics.
- **Interactive Web Interface:** Present recommendations through a user-friendly Streamlit application.
- **Explainable Recommendations:** Where feasible, explain why a talk was recommended.
- **Documentation:** Provide implementation details, evaluation results, and setup instructions.

These are planned capabilities. Features will be marked as implemented as development progresses.

## 🛠️ Technology Stack

| Technology | Purpose |
|---|---|
| Python | Core programming language |
| Pandas | Data manipulation and analysis |
| NumPy | Numerical operations |
| Matplotlib | Data visualization |
| Seaborn | Statistical visualization |
| Scikit-learn | Preprocessing, vectorization, similarity calculations, and model evaluation |
| Jupyter Notebook | Exploratory data analysis and experimentation |
| Streamlit | Interactive web application |
| Git | Version control |
| GitHub | Source code hosting and project documentation |
| Visual Studio Code | Development environment |

The final dependencies will be documented in `requirements.txt` as implementation progresses.

## 🧠 Recommendation Approach

The project will investigate the following approaches.

### 1. Content-Based Filtering

Analyze talk metadata, tags, and transcript content to identify talks similar to a user's selected interests or previously liked talks.

Potential techniques include:

- TF-IDF vectorization
- Cosine similarity
- Text preprocessing
- Metadata-based feature engineering

### 2. Collaborative Filtering

Investigate collaborative filtering if suitable user–item interaction data, such as ratings or watch history, is available.

The availability and quality of such data will determine whether this approach can be implemented meaningfully.

### 3. Hybrid Recommendations

A hybrid approach may combine content-based and collaborative signals if the available data supports both.

The final recommendation strategy will be selected based on data availability, recommendation quality, and evaluation results.

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

**Note:** `requirements.txt` and the implementation files will be added as development progresses. The dataset files shown above are stored locally and are not currently included in the Git repository.

## 📊 Dataset

The project currently uses two CSV files:

- `ted_main.csv` — TED Talks metadata.
- `transcripts.csv` — TED Talks transcript data.

The files were obtained through Kaggle.

Before distributing these datasets, their original sources and licensing conditions must be verified. The CSV files are therefore excluded from version control.

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

Once `requirements.txt` has been created and finalized, install the project dependencies using:

```powershell
python -m pip install -r requirements.txt
```

### 6. Prepare the Dataset

Obtain the required dataset files from the verified source and place them in the local `data/` directory.

Ensure that the filenames match those expected by the project code.

**Important:** The dataset files are not downloaded automatically when cloning this repository.

## 🗺️ Implementation Roadmap

The project follows the four milestones specified in the internship project document.

### Milestone 1 — Data Collection and Exploration

- [ ] Verify dataset sources and licensing.
- [ ] Inspect dataset structure and data types.
- [ ] Analyze missing values and inconsistencies.
- [ ] Perform exploratory data analysis.
- [ ] Preprocess transcripts, tags, and metadata.
- [ ] Generate initial visualizations and summary statistics.

### Milestone 2 — Feature Engineering and Recommendation Engine

- [ ] Select and document text vectorization techniques.
- [ ] Generate numerical representations of talk content.
- [ ] Calculate content similarity scores.
- [ ] Investigate collaborative filtering if suitable interaction data is available.
- [ ] Develop and compare suitable recommendation strategies.
- [ ] Document model design and implementation decisions.

### Milestone 3 — Evaluation

- [ ] Define an appropriate evaluation strategy.
- [ ] Evaluate recommendations using suitable metrics.
- [ ] Investigate Precision, Recall, NDCG, and Mean Average Precision where applicable.
- [ ] Compare recommendation approaches.
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

- [x] Created the local project directory.
- [x] Created the Python virtual environment.
- [x] Installed and verified the initial Python libraries.
- [x] Obtained the TED Talks dataset.
- [x] Created the `data/`, `notebooks/`, and `src/` directories.
- [x] Initialized the local Git repository.
- [x] Configured `.gitignore`.
- [x] Created the initial project README.
- [ ] Verify dataset licensing and document download instructions.
- [ ] Complete dataset inspection and exploratory data analysis.
- [ ] Implement the recommendation engine.
- [ ] Evaluate recommendation quality.
- [ ] Deploy the Streamlit application.

Progress will be updated as each component is implemented and verified.

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
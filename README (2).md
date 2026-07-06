# 🍽️ Zomato Restaurant EDA

An exploratory data analysis (EDA) project on Zomato restaurant listing data — data cleaning,
6 core business questions, 2 extended analytical questions, and 2 bonus visualizations.

## 📊 What's inside

- **Data cleaning** — parsing the `rate` column (`4.1/5` → `4.1`), handling missing values and duplicates
- **Q1–Q6** — the core business questions (restaurant type popularity, votes, rating distribution, spending, order-mode ratings, offline vs online heatmap)
- **Q7 (new)** — correlation between votes and rating
- **Q8 (new)** — top 10 highest-rated restaurants, filtered for a reliable minimum vote count
- **Bonus** — scatter plot (cost vs rating) and pie chart (restaurant type share)

## 🗂️ Repo structure

```
.
├── Zomato_EDA_Project.ipynb   # main notebook
├── zomato_data.csv            # dataset
├── requirements.txt           # Python dependencies
└── README.md
```

## ▶️ Run it in Google Colab

1. Open [Google Colab](https://colab.research.google.com/)
2. `File → Open notebook → GitHub` tab, paste this repo's URL, and select `Zomato_EDA_Project.ipynb`
   (or use the badge below once you've pushed to your own repo)
3. In the **Load Data** section, either:
   - Uncomment the `google.colab.files.upload()` cell and upload `zomato_data.csv` manually, **or**
   - Point `GITHUB_RAW_URL` at your own repo's raw CSV link
4. Run all cells: `Runtime → Run all`

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/<your-username>/<your-repo>/blob/main/Zomato_EDA_Project.ipynb)

*(replace `<your-username>/<your-repo>` above once it's on GitHub)*

## 💻 Run it locally

```bash
git clone https://github.com/<your-username>/<your-repo>.git
cd <your-repo>
pip install -r requirements.txt
jupyter notebook Zomato_EDA_Project.ipynb
```

## 🛠️ Tech stack

- Python, pandas, numpy
- matplotlib, seaborn

## 📌 Key findings

| Question | Finding |
|---|---|
| Most common restaurant type | Dining |
| Most-voted restaurant type | Dining |
| Typical rating range | 3.5 – 4.0 |
| Typical cost for two | ~₹300 |
| Better-rated order mode | Online |
| Type with most offline orders | Dining (Cafes lean online) |
| Votes vs rating | Positive, moderate correlation |

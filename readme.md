# 🚀 MLOps Project with Git & DVC

## 📌 Overview

This project demonstrates a simple **MLOps pipeline** using **Git** and **DVC (Data Version Control)**.
It shows how to manage machine learning workflows with proper versioning of **code, data, and models**.

---

## 🎯 Objectives

* Track code using Git 🧠
* Track data and models using DVC 📦
* Build a reproducible ML pipeline 🔄
* Follow industry-level MLOps practices 🚀

---

## 🛠️ Tech Stack

* Python 🐍
* Scikit-learn 🤖
* Git 🔧
* DVC 📦

---

## 📂 Project Structure

```
mlops-project/
│
├── data/
│   └── raw/
│       └── iris.csv.dvc
│
├── models/
│   └── model.pkl.dvc
│
├── src/
│   ├── load_data.py
│   └── train.py
│
├── dvc.yaml
├── dvc.lock
├── .gitignore
└── README.md
```

---

## ⚙️ Workflow

### 1️⃣ Load Data

```bash
python src/load_data.py
```

### 2️⃣ Track Data with DVC

```bash
dvc add data/raw/iris.csv
git add .
git commit -m "track data"
```

### 3️⃣ Train Model

```bash
python src/train.py
```

### 4️⃣ Create Pipeline

```bash
dvc stage add -n train \
-d src/train.py \
-d data/raw/iris.csv \
-o models/model.pkl \
python src/train.py
```

### 5️⃣ Reproduce Pipeline

```bash
dvc repro
```

---

## 🔁 Reproducibility

This project ensures:

* Same results every time
* Easy collaboration
* Version control for ML assets

---

## 🧠 Key Learnings

* Difference between Git and DVC
* Data & model versioning
* Pipeline automation
* Real-world MLOps workflow

---

## 🚀 Future Improvements

* Add MLflow for experiment tracking 📊
* Integrate CI/CD with GitHub Actions ⚙️
* Deploy model using Docker & AWS ☁️

---

## 💼 Author

**Akash Goli**
B.Tech Student | Aspiring MLOps & Cloud Engineer

---

## ⭐ If you like this project

Give it a ⭐ on GitHub and connect with me!

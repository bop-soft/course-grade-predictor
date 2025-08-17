# Course Grade Predictor: Machine Learning
I trained a RandomForestClassifier on a dataset to predict letter grades.
I calculated feature importances, showing which parts (e.g., quizzes, assignments) are most influential in predicting final grades.
We can apply this model to incomplete course data.
You’ll get predictions like: “Based on your current performance, you're on track for a B+.”

I also trained a RandomForestRegressor on a dataset to predict number grades.
I converted predicted numeric grades back into letter grades using the preferred grading scale.

---

## ✅ Step 1: Create a Project Directory (Optional but Recommended)

Open your terminal:

```bash
mkdir course-grade-predictor
cd course-grade-predictor
```

---

## ✅ Step 2: Create a Virtual Environment

```bash
python3 -m venv venv
```

* This creates a folder named `venv` containing your isolated Python environment.

---

## ✅ Step 3: Activate the Virtual Environment

```bash
source venv/bin/activate
```

You should now see `(venv)` at the start of your terminal prompt, that means it’s active.

---

## ✅ Step 4: Upgrade pip and Install Required Packages

```bash
pip install --upgrade pip
pip install pandas scikit-learn jupyter
```

---

## ✅ Step 5: Add Your Dataset

Move your CSV dataset (`refined_course_dataset.csv`) into your project directory:

```bash
mv /path/to/refined_course_dataset.csv .
```

Use the actual path to your file.

---

## ✅ Step 6: Launch Jupyter Notebook

```bash
jupyter notebook
```

* This will open Jupyter Notebook in your default web browser.
* Inside the browser interface:

  * Navigate to your project folder.
  * Click **New > Python 3 (ipykernel)** to create a new notebook.

---

## ✅ Step 7: Paste the Model Code

* Copy the full Python code into a cell in the new notebook.
* Run the cell to train the model and make predictions.

---

## ✅ Step 8: (Optional) Freeze Your Environment for Reuse

To save your environment for later use:

```bash
pip freeze > requirements.txt
```

Then you (or others) can recreate it with:

```bash
pip install -r requirements.txt
```

---

## ✅ Step 9: Deactivate the Virtual Environment When Done

```bash
deactivate
```

This returns you to your system’s global Python environment.

---

## Troubleshooting

* If `jupyter` isn't recognized: Make sure you're in the virtual environment and run `pip install jupyter`.
* If the notebook doesn't open: Visit `http://localhost:8888` manually in your browser.
* If you want VS Code integration: install the Python extension and use "Select Interpreter" to choose your `venv`.

---

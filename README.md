# Workshop 1: Tools and Libraries

Welcome to the introductory workshop for **Machine Learning, Deep Learning & Security** (`MLDLS`).

This workshop serves as a pilot session designed to achieve two main goals:

1. **Technical Validation:** Verify that your local Python environment, dependencies, and core libraries (`NumPy`, `Pandas`, `Matplotlib`, `Seaborn`) are correctly configured.
2. **Workflow & Grading Assessment:** Familiarize you with the automated grading system (`nbgrader`) and the Git submission workflow (`upstream` / `origin`) that will be used for all remaining sessions throughout the semester.

To test your environment, this session applies the **Spam Classification** example covered during the introductory lecture.

---

## 🎯 Objectives

By completing this workshop, you will:

- Verify your local Python runtime environment and library versions.
- Master the **Git submission pipeline** (pulling updates from `upstream` and pushing solutions to your private `origin`).
- Respond using `nbgrader` autograded cells.
- Implement matrix operations ($z = S\theta + b$), sigmoid vector operations, and binary thresholding for spam detection using `NumPy`.

---

## 🛠️ Environment & Workflow Instructions

You can complete this notebook locally on your computer or in Google Colab. Choose the setup that applies to you below.

### Option A: Local Setup (VS Code / JupyterLab)

#### 1. One-Time Setup (If not already done)
Link your private repository to the course central distribution repository (`upstream`):

```bash
git remote add upstream https://github.com/ING4-MLDLS/Workshop_1_Tools_and_Libraries.git
```

#### 2. Fetching Workshop Files
To fetch and merge the latest workshop updates into your local working branch:

```bash
git fetch upstream
git merge upstream/main --allow-unrelated-histories -m "Fetch Workshop 1"
```

---

### Option B: Google Colab Setup

If you prefer using **Google Colab**, follow these steps to work on and save your assignment:

1. **Open the Notebook in Colab:**
   - Go to [Google Colab](https://colab.research.google.com/).
   - Select the **GitHub** tab.
   - Enter your private repository URL or `ING4-MLDLS/coursework-2026`.
   - Select `Workshop1_tools_and_libraries/Workshop1.ipynb`.

2. **Save Your Changes directly to GitHub:**
   - As you complete exercises, go to **File $\rightarrow$ Save a copy in GitHub**.
   - Select your private repository (`origin`).
   - Ensure the file path remains strictly: `Workshop1_tools_and_libraries/Workshop1.ipynb`.
   - Add a commit message (e.g., `"Update Workshop 1 solutions"`) and click **OK**.

---

## 📂 Workshop Contents

```text
Workshop1_tools_and_libraries/
├── README.md                            <-- This file
├── Workshop_1_Tools_and_Libraries.pdf   <-- The main document
└── Workshop_1_Tools_and_Libraries.ipynb <-- The notebook to complete and submit
```

---

## ⚠️ Essential Rules for Autograding

Because your work will be collected and graded automatically using `nbgrader`, you must adhere to the following rules:

1. **Keep the Notebook Name Intact:** Do **NOT** rename `Workshop_1_Tools_and_Libraries.ipynb`.
2. **Write Code Only in Designated Areas:** Insert your solutions strictly between the solution comments:
   ```python
   ### BEGIN SOLUTION
   # Your code here
   ### END SOLUTION
   ```
3. **Do NOT Alter or Delete Test Cells.**
4. **Test Before Submitting:** Run all test cells locally in Jupyter. Ensure you execute `Kernel -> Restart & Run All` to verify there are no hidden state issues or out-of-order execution bugs.

---

## 🚀 How to Submit Your Work

1. Save your notebook in JupyterLab / Jupyter Notebook.
2. Open your terminal in your repository folder.
3. Commit and push your changes to your private repository (`origin`):

```bash
git add Workshop1_tools_and_libraries/Workshop1.ipynb
git commit -m "Submit Workshop 1: Setup and Spam Classification"
git push origin main
```

> ⏰ **Submission Deadline:** Ensure your final commit is pushed to your `main` branch before the announced deadline. Automatic collection will run directly on your private GitHub repositories.

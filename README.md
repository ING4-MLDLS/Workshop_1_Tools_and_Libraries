# Workshop_1_Tools_and_Libraries

Welcome to the introductory workshop for Machine Learning, Deep Learning & Security (MLDLS).

This workshop serves as a pilot session designed to achieve two main goals:

1. Technical Validation: Verify that your Python environment, dependencies, and core libraries (NumPy, Pandas, Matplotlib, Seaborn) are correctly configured.

2. Workflow & Grading Assessment: Familiarize you with the automated grading system (nbgrader) and the Git submission workflow (upstream / origin) that will be used for all remaining practical sessions throughout the semester.

To test your environment, this session applies the Spam Classification example covered during the introductory lecture, framed within an IT security context.

## Objectives

By completing this workshop, you will:

* Verify your local Python runtime environment and library versions.

* Master the Git submission pipeline (pulling updates from upstream and pushing solutions to your private origin).

* Respond using nbgrader autograded cells.

* Implement matrix operations ($z = S\theta + b$), sigmoid vector operations, and binary thresholding for spam detection using NumPy.

## Repository Contents

Your template repository contains the following files:

```
Workshop_1_Tools_and_Libraries/
├── README.md                              <-- This instruction file
├── Workshop_1_Tools_and_Libraries.pdf     <-- The official workshop subject & statements
├── Workshop_1_Tools_and_Libraries.ipynb   <-- The notebook to complete and submit
└── logins.csv                             <-- Authentication log dataset for future exercises

```

## Environment & Setup Instructions

You can complete this assignment locally using JupyterNotebook, or online using Google Colab.

### 1. Local Setup (JupyterNotebook / JupyterLab)

1. Link Central Template Repository (Upstream):
   Open your terminal in your local repository folder and run:

   ```
   git remote add upstream https://github.com/ING4-MLDLS/Workshop_1_Tools_and_Libraries.git
   
   ```

2. Fetch Assignment Files:
   Retrieve the workshop files into your working branch:

   ```
   git fetch upstream
   git merge upstream/main --allow-unrelated-histories -m "Fetch Workshop 1 template"
   
   ```

3. Open Notebook:
   Launch JupyterLab or VS Code and open `Workshop_1_Tools_and_Libraries.ipynb`.

### 2. Google Colab Setup

1. Open in Google Colab:

   * Go to Google Colab.

   * Click on the GitHub tab.

   * Enter the repository URL: `https://github.com/ING4-MLDLS/Workshop_1_Tools_and_Libraries.git`.

   * Select `Workshop_1_Tools_and_Libraries.ipynb`.

2. Save Work directly to GitHub:

   * As you complete your code, go to File -> Save a copy in GitHub.

   * Select your private repository (origin).

   * Ensure the file path remains exactly: `Workshop_1_Tools_and_Libraries.ipynb`.

   * Add a commit message (e.g., "Update Workshop 1 answers") and click OK.

## Rules for Answer Insertion & Autograding

Your answers will be collected and evaluated automatically using nbgrader. Please follow these mandatory rules:

1. Keep Filenames Intact: Do NOT rename `Workshop_1_Tools_and_Libraries.ipynb`.

2. Insert Answers in Dedicated Cells: Write your code strictly inside the designated solution blocks:

   ```
   # Your code here
   
   ```

3. Do NOT Delete Test Cells: Read-only test cells (containing assert or hidden tests) are used by the automated evaluator. Do not modify or delete them.

4. Kernel Restart Check: Before submitting, select Kernel -> Restart & Run All to verify that your notebook executes sequentially without errors.

## Submission Process

Once all exercises are completed and verified:

1. Save your notebook file (`Workshop_1_Tools_and_Libraries.ipynb`).

2. Open your terminal in your local repository directory.

3. Commit and push your work to your private student repository (origin):

```
git add Workshop_1_Tools_and_Libraries.ipynb
git commit -m "Submit Workshop 1: Tools and Libraries"
git push origin main

```

Important: Ensure your final code is pushed to your main branch before the submission deadline. Automatic collection scripts will pull directly from your private GitHub repository.

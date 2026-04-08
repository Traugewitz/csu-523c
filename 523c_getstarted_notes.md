We are going to do this in a very specific order:



1. create the GitHub repository
2. clone it to your computer
3. open it as an RStudio Project
4. add the lab .qmd file
5. make sure Quarto is working
6. render the file
7. commit and push to GitHub
8. later, turn on GitHub Pages



Why it matters



**This class is not just teaching you R code. It is teaching you a reproducible workflow, which means:**



1. your files are organized
2. your code lives in one project folder
3. GitHub stores your work safely
4. Quarto turns your code and writing into a webpage







**Part 1: Create the GitHub repository**



1. Go to GitHub in your browser and log in.



**Then:**



1. Click the + in the top right
2. Choose New repository
3. Repository name: csu-523c
4. Set it to Public unless your instructor said otherwise
5. Check Add a README file
6. Click Create repository the kind of workflow environmental data scientists use in real work.

\--------------------------------------------------------------------------------------------------------------------------

**Absolutely. Let’s make this easy to start and reusable so you are not staring at a blank file.**



Goal



Set up Lab 2 in your csu-523c repository by creating a clean Quarto starter script for lab-02.qmd.



Why this matters



The hardest part of coding projects is often not the coding itself. It is:



knowing what file to make

knowing what goes at the top

knowing what packages to load

knowing how to organize the work

\-----------------------------------------------------------------------------------------------------------------

**GitHub repo** → RStudio project → Quarto file → render → push → **GitHub Pages**



csu-523c/

│

├── lab-01.qmd

├── lab-02.qmd

├── lab-03.qmd

│

├── data/          ← (optional: datasets)

├── docs/          ← (auto-created by Quarto)

├── images/        ← (optional: figures)

│

├── \_quarto.yml

├── README.md

└── csu-523c.Rproj



This starter script gives you a repeatable structure for ESS 523C labs so you can stop reinventing the setup every time.



What you should do first

**Step 1: Open your csu-523c project in RStudio**



You want to be inside the correct project folder.



You should see your files in the Files pane and your project name at the top of RStudio.



Step 2: Create a new Quarto file



In RStudio:



File

New File

Quarto Document



Name it





Short answer: \*\*No — do NOT create a new project for every lab.\*\*



That would actually make your life harder.



\---



\# 🎯 Goal



Understand how to organize your work for ESS 523C so you:



\* stay organized

\* avoid GitHub chaos

\* build a clean portfolio



\---



\# 🧠 The right structure (what your instructor expects)



You should have \*\*ONE GitHub repository + ONE RStudio project\*\* for the entire course:



```text

csu-523c/

│

├── lab-01.qmd

├── lab-02.qmd

├── lab-03.qmd

│

├── data/          ← (optional: datasets)

├── docs/          ← (auto-created by Quarto)

├── images/        ← (optional: figures)

│

├── \\\_quarto.yml

├── README.md

└── csu-523c.Rproj

```



\---



\# ❌ What NOT to do



Do NOT do this:



```text

lab-01-project/

lab-02-project/

lab-03-project/

```



\### Why this is a bad idea



\* ❌ Too many repos to manage

\* ❌ GitHub Pages becomes messy

\* ❌ You lose the “portfolio” structure

\* ❌ Harder for your instructor to grade



\---



\# ✅ What you SHOULD do



Use:



> \\\*\\\*One project → multiple lab files\\\*\\\*



Each week:



\* create a new `.qmd` file

\* keep everything inside the same repo



\---



\# 🔁 Your weekly workflow (this is your system)



Every lab:



\## Step 1 — Open your project



```text

csu-523c.Rproj

```



\## Step 2 — Pull latest version



```bash

git pull

```



\## Step 3 — Create new file



```text

lab-03.qmd

```



\## Step 4 — Do your work



\## Step 5 — Render



```bash

quarto render lab-03.qmd

```



\## Step 6 — Push



```bash

git add -A \\\&\\\& git commit -m "lab 3 complete" \\\&\\\& git push

```



\---



\# 🌐 What this creates (this is the payoff)



Your GitHub Pages site becomes:



```text

https://USERNAME.github.io/csu-523c/

```



With pages like:



\* `/lab-01.html`

\* `/lab-02.html`

\* `/lab-03.html`



👉 This is literally your \*\*public portfolio\*\*



\---



\# 🔥 Why this is powerful (career connection)



This setup shows employers:



\* you can manage a repo

\* you understand reproducible workflows

\* you can publish analysis results

\* you organize work professionally



That’s exactly what environmental data roles require.



\---



\# ⚠️ One thing to double-check



Make sure your `\\\_quarto.yml` includes:



```yaml

website:

\&#x20; output-dir: docs

```



👉 This ensures all labs render into `/docs`, which GitHub Pages uses.



\---



\# 🧩 Mental model (this will help it stick)



Think of it like this:



\* \*\*Repo = your notebook\*\*

\* \*\*Each lab = a chapter\*\*

\* \*\*Quarto = your publishing tool\*\*

\* \*\*GitHub Pages = your website\*\*



\---



\# 💬 Bottom line



👉 One repo

👉 One project

👉 One growing portfolio



\---



\# 👉 Next step



If you want to level this up, I can help you:



\* turn your repo into a \*\*clean Quarto website homepage\*\*

\* add navigation (Lab 1 → Lab 2 → Lab 3)

\* make it look like a professional portfolio



Or we can jump straight into the \*\*first spatial step in Lab 2\*\*.


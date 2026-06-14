# 🎯 30-DAY DiPaQ ADMISSION PLAN
### Goal: 3 GitHub repos + killer application for M1 DiPaQ Paris-Saclay
### Daily time: 3 hours max

---

## 📦 FINAL DELIVERABLES
- `parallel-matrix-mul` – GitHub repo (C + OpenMP, speedup graph)
- `simple-mapreduce` – GitHub repo (Python, multiprocessing, timing)
- `grover-search-qiskit` – GitHub repo (Qiskit notebook, Grover histogram)
- Pièce Libre PDF (3 projects portfolio)
- Motivation letter (DiPaQ-specific)
- CV (with projects)
- Recommendation letter (algorithms professor)
- All transcripts scanned

---

## 🔥 WEEK 1: PARALLEL MATRIX MULTIPLICATION (OpenMP)
### Repo: `parallel-matrix-mul`

| Day | Task |
|-----|------|
| 1 | Install GCC (or WSL on Windows). Read [LLNL OpenMP tutorial](https://hpc.llnl.gov/tuts/openmp/) — only "Introduction" and "Parallel Regions". Write a C program: spawn 4 threads, each prints "Hello from thread X". Compile with `gcc -fopenmp`. Run it. |
| 2 | Write serial matrix multiplication. Two 500×500 matrices. Nested loops. Time it with `omp_get_wtime()`. |
| 3 | Parallelize outer loop with `#pragma omp parallel for`. Run with 1, 2, 4 threads. Record times. |
| 4 | Add `collapse(2)`. Try N=1000, N=1500. Record all times in a table. |
| 5 | Generate speedup bar chart (Python matplotlib or Excel). X-axis: threads. Y-axis: time. Add ideal speedup line. Save as `speedup.png`. |
| 6 | Write README.md: description, compile/run instructions, results table, graph, one sentence on Amdahl's Law. Push to GitHub. **Repo 1 DONE.** |
| 7 | **REST.** Do nothing. |

---

## 🔥 WEEK 2: SIMPLE MAPREDUCE ENGINE (Python)
### Repo: `simple-mapreduce`

| Day | Task |
|-----|------|
| 8 | Download free book from [Project Gutenberg](https://www.gutenberg.org/) as `.txt`. Watch any 10-min YouTube video "MapReduce explained". |
| 9 | Write `mapper()`: takes text chunk, splits into words, returns list of `(word, 1)` tuples. |
| 10 | Write `reducer()`: takes list of `(word, count)`, sums counts per word, returns dict. |
| 11 | Single-threaded pipeline: read file → map → shuffle → reduce. Print top 10 words. |
| 12 | Convert mapper to `multiprocessing.Pool`. Split file into chunks, map each chunk in parallel. Merge results. |
| 13 | Add simple shuffle: group mapped pairs by word hash before reducing. Time single vs multi-process. Print comparison. |
| 14 | Write README.md: explain map/shuffle/reduce, timing comparison, how to run. Push to GitHub. **Repo 2 DONE.** |

---

## 🔥 WEEK 3: GROVER'S SEARCH (Qiskit)
### Repo: `grover-search-qiskit`

| Day | Task |
|-----|------|
| 15 | Install Qiskit: `pip install qiskit`. Open [Qiskit textbook "Getting Started"](https://qiskit.org/textbook/ch-prerequisites/qiskit.html). Run Bell state example. Tweak and rerun. |
| 16 | Open [Qiskit textbook "Grover's Algorithm"](https://qiskit.org/textbook/ch-algorithms/grover.html). Read sections 1–3 (skip math derivations, read bold words). Copy example code for 3 qubits. Run on `qasm_simulator`. See histogram. |
| 17 | Modify oracle: mark different state (e.g., `|110⟩`). Rerun. Confirm histogram peaks at new state. |
| 18 | Create Jupyter notebook. Add markdown explaining: qubit, superposition, oracle, diffusion. Keep it simple. |
| 19 | In notebook: show code → run → histogram. Label everything. Export as `.ipynb`. |
| 20 | Write README.md: install, run, what output means. Push to GitHub. **Repo 3 DONE.** |
| 21 | **REST.** Half day off. |

---

## 🔥 WEEK 4: POLISH + APPLICATION PACKAGE

| Day | Task |
|-----|------|
| 22 | **Repo cleanup.** Check all 3 repos: public? Clean README? Instructions? Results visible? Fix anything. |
| 23 | **Create Pièce Libre PDF.** One page per project: title, 2-sentence description, screenshot (speedup graph / MapReduce output / Grover histogram), GitHub link. Combine into single PDF. |
| 24 | **Write Motivation Letter – Draft 1.** (1) Introduction: who you are, Algerian CS student. (2) Why DiPaQ: mention parallel, distributed, quantum. (3) Proof: 18.67 in algorithms + 3 projects (name them). (4) Future: researcher/engineer in these fields. |
| 25 | **Revise letter.** Cut fluff. Check grammar. Get feedback. |
| 26 | **Prepare CV.** Education (Bac, L1, L2 — mention 18.67 algo). Projects (3 repos + links). Skills (C, Python, OpenMP, Qiskit, Git, multiprocessing). Languages (Arabic, French, English). Save as PDF. |
| 27 | **Request recommendation letter.** Email Algorithms professor. Explain DiPaQ, your projects, why it matters. |
| 28 | **Scan all documents.** Transcripts (Bac, L1, L2), CV, motivation letter, Pièce Libre, recommendation letter. All PDF. Name cleanly: `Nom_Prenom_CV.pdf`. |
| 29 | **UPLOAD EVERYTHING.** Inception or Mon Master. Check every field. Submit. |
| 30 | **Buffer day.** Fix issues or celebrate. Done. |

---

## ⚠️ IF YOU FALL BEHIND
- Week 1 is non-negotiable. One parallel project = proof you're ready.
- Week 2: even single-threaded MapReduce with parallelism plan is okay.
- Week 3: Qiskit textbook example + your markdown explanation is enough.
- **One solid project + great letter > three rushed projects.**

---

## 🔗 KEY RESOURCES
- OpenMP: https://hpc.llnl.gov/tuts/openmp/
- Qiskit Getting Started: https://qiskit.org/textbook/ch-prerequisites/qiskit.html
- Qiskit Grover's Algorithm: https://qiskit.org/textbook/ch-algorithms/grover.html
- Project Gutenberg (free texts): https://www.gutenberg.org/

---

**Start Day 1 tomorrow. Install GCC. Go.**

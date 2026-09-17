# Qiskit 101: Hands-on Quantum Computing with Qiskit

[![Qiskit](https://img.shields.io/badge/Qiskit-2.5.2-6929C4)](https://qiskit.org/)
[![Python](https://img.shields.io/badge/Python-3.10%2B-3776AB)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A five-lab, competency-based introduction to quantum computing with Qiskit. The course begins with Google Colab setup, develops single- and multi-qubit circuit skills, progresses to IBM Quantum hardware, and concludes with algorithms, noise analysis, and a mini-project.

**Instructor:** Prof. Arvind W. Kiwelekar, Department of Computer Engineering, Dr. Babasaheb Ambedkar Technological University (DBATU), Lonere, Maharashtra, India.

## Course pathway

| Lab | Topic | Primary outcome | Notebook | Slides |
|---|---|---|---|---|
| 00 | Setup and environment | Configure Qiskit in Google Colab and verify the installation | [Notebook](notebooks/00_setup.ipynb) · [Open in Colab](https://colab.research.google.com/github/akiwelekar/qiskit-101/blob/main/notebooks/00_setup.ipynb) | [Slides](Slides/Lab_00_.pptx.pdf) |
| 01 | Single-qubit computing | Prepare, transform, measure, and visualize single-qubit states | [Notebook](notebooks/01_single_qubit.ipynb) · [Open in Colab](https://colab.research.google.com/github/akiwelekar/qiskit-101/blob/main/notebooks/01_single_qubit.ipynb) | [Slides](Slides/Lab01.pptx.pdf) |
| 02 | Multi-qubit computing | Build multi-qubit circuits and investigate entanglement | [Notebook](notebooks/02_multi_qubit.ipynb) · [Open in Colab](https://colab.research.google.com/github/akiwelekar/qiskit-101/blob/main/notebooks/02_multi_qubit.ipynb) | [Slides](Slides/Lab_02.pptx.pdf) |
| 03 | Circuit to hardware | Transpile and execute circuits on IBM Quantum hardware | [Notebook](notebooks/03_quantum_hardware.ipynb) · [Open in Colab](https://colab.research.google.com/github/akiwelekar/qiskit-101/blob/main/notebooks/03_quantum_hardware.ipynb) | [Slides](Slides/Lab03.pptx.pdf) |
| 04 | Algorithms, noise, and mini-project | Implement a complete workflow and analyze noisy results | [Notebook](notebooks/04_algorithms_noise_project.ipynb) · [Open in Colab](https://colab.research.google.com/github/akiwelekar/qiskit-101/blob/main/notebooks/04_algorithms_noise_project.ipynb) | [Slides](Slides/Lab_04.pptx.pdf) |

## Getting started

The simplest route is to open a notebook using its **Open in Colab** link and run the cells in order. Use the corresponding slide deck before each laboratory session to review the concepts, objectives, and activities. Lab 03 requires an [IBM Quantum](https://quantum.cloud.ibm.com/) account and API token. Never place an API token directly in a notebook or commit it to GitHub.

For local use:

```bash
git clone https://github.com/akiwelekar/qiskit-101.git
cd qiskit-101
python -m venv .venv
source .venv/bin/activate  # Windows: .venv\Scripts\activate
python -m pip install -r requirements.txt
jupyter lab
```

## Recommended learning sequence

Complete the labs in numerical order. Each lab follows a **lecture → hands-on notebook → observation → competency assessment** pattern. Learners should modify circuits, predict results before execution, and record interpretations rather than only running the supplied cells.

## Repository contents

```text
qiskit-101/
├── notebooks/             # Five learner notebooks
├── Slides/                # Lecture/lab presentation decks
│   └── README.md          # Slide guide and notebook mapping
├── docs/                  # Course overview, instructor guide, troubleshooting
├── .gitignore
├── CITATION.cff
├── CODE_OF_CONDUCT.md
├── CONTRIBUTING.md
├── LICENSE
├── README.md
└── requirements.txt
```

## Software versions

The notebooks were prepared with Qiskit 2.5.2, Qiskit Aer 0.17.2, and Qiskit IBM Runtime 0.49.0. Cloud backends and queues change over time; select an available operational backend when reproducing hardware exercises.

## Citation

If you use or adapt this course, please cite it using the repository's `CITATION.cff` file.

## License

This repository is released under the [MIT License](LICENSE).

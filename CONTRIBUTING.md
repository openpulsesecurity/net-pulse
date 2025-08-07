# Contributing to NetPulse

Thank you for your interest in contributing to **NetPulse**! We welcome contributions of all kinds—whether you’re improving documentation, fixing bugs, proposing new features, or helping with testing.

---

## Table of Contents

1. Why Contribute?  
2. Code of Conduct  
3. Getting Started  
4. Reporting Issues  
5. Feature Requests  
6. Development Workflow  
7. Coding Guidelines  
8. Commit Message Format  
9. Pull Request Process  
10. Contact & Support  

---

## 1. Why Contribute?

NetPulse is an open-source, community-driven project. Your contributions will help:

- Accelerate development of new features  
- Improve stability and performance  
- Write and refine documentation  
- Grow and support a welcoming community  

---

## 2. Code of Conduct

By participating in this project, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md). Please read it to ensure a safe and respectful community.

---

## 3. Getting Started

1. Fork the repository on GitLab:  
   `https://gitlab.com/open-pulse-security/net-pulse`  
2. Clone your fork locally:  
   ```bash
   git clone https://gitlab.com/your-username/net-pulse.git
   cd NetPulse
   ```  
3. Create and activate a Python 3.8+ virtual environment:  
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate   # Linux/macOS
   .\.venv\Scripts\activate    # Windows
   ```  
4. Install development dependencies (once `requirements-dev.txt` is added):  
   ```bash
   pip install -r requirements-dev.txt
   ```  
5. (Optional) Set up pre-commit hooks for linting/formatting:  
   ```bash
   pip install pre-commit
   pre-commit install
   ```

---

## 4. Reporting Issues

If you find a bug or run into any problems:

1. Search existing issues to see if it’s already been reported.  
2. If not, open a new issue and include:  
   - A clear, descriptive title  
   - Steps to reproduce the problem  
   - Expected vs. actual behavior  
   - Screenshots or logs, if applicable  

---

## 5. Feature Requests

We welcome ideas for new features! To request a feature:

1. Check the list of open issues/features to avoid duplicates.  
2. Create a new issue with:  
   - A descriptive title  
   - A summary of the proposed feature  
   - Any relevant use cases or sketches  

---

## 6. Development Workflow

We follow a **GitLab flow**:

1. **Branching**  
   - Create a branch per issue or feature:  
     `git checkout -b feat/<short-description>`  
     `git checkout -b fix/<short-description>`  
2. **Work**  
   - Make your changes  
   - Run tests and linters locally  
3. **Commit**  
   - Write clear, concise commit messages (see below)  
4. **Push**  
   - Push your branch to your fork:  
     `git push origin feat/<short-description>`  
5. **Pull Request**  
   - Open a PR against `main` in the upstream repo  
   - Fill out the PR template with details  

---

## 7. Coding Guidelines

- Follow [PEP 8](https://www.python.org/dev/peps/pep-0008/) for Python style.  
- Use meaningful variable and function names.  
- Keep functions short and focused (max ~50 lines).  
- Document public functions and classes with docstrings.  
- For UI code (Tkinter), separate logic from presentation where possible.  
- Write tests for new features/bug fixes.  

---

## 8. Commit Message Format

Use a simple, consistent format:

```
<type>(<scope>): <short description>

<body>

<footer>
```

- **type**: feat, fix, docs, refactor, test, chore  
- **scope**: optional area of the code (e.g., `gui`, `core`, `storage`)  
- **short description**: ≤50 characters  
- **body**: more detailed explanation (wrap at 72 characters)  
- **footer**: issue references, breaking changes, etc.

Example:

```
feat(core): add JSON-based persistence layer

This adds save_data() and load_data() functions to handle
equipment data in JSON format.

Closes #12
```

---

## 9. Pull Request Process

1. Ensure your branch is up to date with `main`.  
2. Run all tests and make sure they pass.  
3. Link related issues in the PR description.  
4. Describe what you’ve done and why.  
5. Request reviews from maintainers.  
6. Address review comments and update your PR.  

---

## 10. Contact & Support

- For general discussion and questions, use GitLab Discussions.  
- For urgent issues, open an issue and tag a maintainer.  
- You can also reach the maintainers via email: code@openpulsesec.org  

---

Thank you for helping make NetPulse better! 🚀  
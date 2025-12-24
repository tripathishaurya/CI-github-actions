🚀 Learning GitHub Actions – CI Workflow

This repository documents my hands-on learning of GitHub Actions, focusing on setting up a Continuous Integration (CI) pipeline from scratch using YAML workflows.

I built, broke, debugged, and fixed the workflow myself — this repo reflects real learning, not paid certificates or dummy automation.

📌 What I Learned

What GitHub Actions are and why they matter in real-world projects

How CI (Continuous Integration) works in practice

Writing and debugging YAML workflows

Understanding:

on: event triggers

jobs, runs-on, and steps

Actions vs shell commands

Running automated tests using pytest

Reading GitHub Actions logs to debug failures

⚙️ CI Workflow Overview

The workflow automatically runs when:

Code is pushed to main

A pull request is opened against main

Current workflow steps:

Checkout repository code

Set up Python environment

Install dependencies

Run test cases using pytest

🧠 Key Concepts Understood

Event-driven automation (push, pull_request)

Runner environments (ubuntu-latest)

Versioned actions (actions/checkout, actions/setup-python)

Fail-fast behavior of CI pipelines

Why CI fails when:

Tests don’t exist

Paths are incorrect

Dependencies are missing

Triggers are misconfigured

🛠️ Workflow File

The CI configuration lives here:

.github/workflows/ci.yaml


This file defines when the workflow runs and what steps are executed.

✅ Why This Matters

CI is a core industry practice.
Through this repo, I learned how teams:

Prevent broken code from being merged

Maintain code quality automatically

Build trust in deployments and collaboration

This workflow is intentionally simple but production-aligned.

🔮 Future Improvements

Add requirements.txt

Cache dependencies for faster builds

Run CI on multiple Python versions

Add linting (flake8 / black)

Expand test coverage

🧑‍💻 Author

Shaurya
Learning ML, AI Engineering, and practical software engineering
Focused on building real skills, not shortcuts.

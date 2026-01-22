# Apply Advanced GitHub Copilot Techniques

This repository contains the exercise materials and sample code for applying **advanced GitHub Copilot techniques** within a Python web application that exposes an interactive API. The exercises help you experience how to use GitHub Copilot (including Copilot Chat and Agent modes) to implement new endpoints and tests in a real-world scenario. ([GitHub][1])

## Table of Contents

* **About**
* **Prerequisites**
* **Exercise Overview**
* **Getting Started**
* **Tasks**
* **Testing**
* **License**
* **Contributing**
* **Security**
* **Acknowledgements**

---

## About

This repository is based on the Microsoft Learn project **mslearn-advanced-copilot**, which demonstrates how to use GitHub Copilot in advanced ways within a Python project to add functionality and write tests. You will implement API routes, interact with Copilot Chat prompts, and refine results using notionally “agent” workflows. ([GitHub][1])

---

## Prerequisites

Before working with this repository, ensure you have the following:

* A **GitHub Copilot** subscription or service enabled (GitHub Copilot, Copilot Chat). ([GitHub][1])
* GitHub **Codespaces** (optional but recommended for seamless experience). ([GitHub][1])
* Python 3.9+ installed locally if not using Codespaces. ([GitHub][1])
* Familiarity with basic Python and FastAPI (or equivalent web frameworks). ([GitHub][1])

---

## Exercise Overview

This repository hosts a sample Python web application (Travel Weather API) that provides historical weather-related endpoints. Your goals include:

1. **Implementing new API routes** (e.g., listing cities per country).
2. **Creating tests** using pytest and Copilot assistance.
3. **Using Copilot Chat** (inline and workspace prompts) to generate documentation or helpers.
4. **Exploring Copilot’s advanced techniques** to iterate on and refine your code. ([GitHub][1])

---

## Getting Started

### Clone the Repository

Clone it locally or open it directly in GitHub Codespaces:

```bash
git clone https://github.com/BrunoGil-AS/mslearn-advanced-copilot.git
cd mslearn-advanced-copilot
```

### Install Dependencies

Using a Python virtual environment:

```bash
python -m venv venv
source venv/bin/activate   # macOS / Linux
venv\Scripts\activate      # Windows
pip install -r requirements.txt
```

---

## Tasks

### 1. Add a New API Route

In `main.py`, create a new route such as:

```python
@app.get("/countries/{country}")
def cities(country: str):
    return list(data[country].keys())
```

Use GitHub Copilot inline prompts (e.g., `ctrl+i` or `cmd+i`) to help generate route code. ([GitHub][1])

---

### 2. Write Tests

Create a test function in `test_main.py` that verifies the new route works for specific countries like Spain. Use pytest:

```bash
pytest
```

Then ask Copilot Chat assistant to help create or refine the test. ([GitHub][1])

---

### 3. Use an Agent to Generate Documentation

In Copilot Chat, try workspace-level prompts (e.g., `@workspace help me to use an agent to write the project documentation on how to run it`). ([GitHub][1])

---

## Testing

Run the test suite using:

```bash
pytest
```

Ensure that all tests pass and add new ones as you implement features. ([GitHub][1])

---

## License

This repository uses **multiple licenses**:

* Source documentation and exercise content is under **Creative Commons Attribution 4.0 (CC-BY-4.0)**. ([GitHub][1])
* Code samples are under the **MIT License**. ([GitHub][1])

Refer to the respective `LICENSE` and `LICENSE-CODE` files for details. ([GitHub][1])

---

## Contributing

Contributions are welcome. Please read the **CONTRIBUTING.md** file for guidelines on submitting issues and pull requests. ([GitHub][1])

---

## Security

See the **SECURITY.md** file for details on our security policy and reporting vulnerabilities. ([GitHub][1])

---

## Acknowledgements

This repository is generated from MicrosoftDocs’ **mslearn-advanced-copilot** materials and demonstrates how to use GitHub Copilot to build and extend a Python API project interactively with advanced AI-assisted coding workflows. ([GitHub][1])



# LeetCode Solutions

Welcome to my LeetCode solutions repository. Here you will find my solutions to various LeetCode problems, categorized by difficulty.

## Structure

- `solutions/` contains directories for each problem, organized by difficulty.
- Each problem directory includes:
  - `solution.py`: The Python solution.
  - `test_solution.py`: Test cases for the solution.
  - `README.md`: A detailed walkthrough of the problem and solution.

## File Naming Convention

To maintain clarity and consistency, the files are named following this convention:

- Solution Script: `<problem-number>-<problem-name>-<difficulty>.py`
- Test Script: `test_<problem-number>-<problem-name>-<difficulty>.py`
- Problem Description (README): `README.md`
  - This file is inside a directory specific to the problem, which includes the problem number and name.

## How to Use

1. Clone the repository.
2. Navigate to the desired problem directory.
3. Run the solution script or test script.

## Table of Contents

- [Easy Problems](#easy-problems)
- [Medium Problems](#medium-problems)
- [Hard Problems](#hard-problems)

### Easy Problems

- ...

### Medium Problems

- ...

### Hard Problems

- ...

## Steps to Add a New Problem (for PowerShell)

1. **Create the necessary directories and files**:

   ```powershell
   # Create the necessary directories
   New-Item -ItemType Directory -Path solutions\easy\<problem-number>-<problem-name>

   # Create the solution file
   New-Item -ItemType File -Path solutions\easy\<problem-number>-<problem-name>\<problem-number>-<problem-name>-easy.py

   # Create the test file
   New-Item -ItemType File -Path solutions\easy\<problem-number>-<problem-name>\test_<problem-number>-<problem-name>-easy.py

   # Copy the README template to the new problem directory
   Copy-Item -Path README_TEMPLATE.md -Destination solutions\easy\<problem-number>-<problem-name>\README.md
   ```

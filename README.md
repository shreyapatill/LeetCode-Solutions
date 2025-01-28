# Competitive Coding Solutions

Welcome to my **competitive coding** solutions repository! Here you will find solutions for **LeetCode** and **Work@Tech** problems in various programming languages (such as Python, C++, Java, etc.), neatly organized by difficulty.

## Repository Structure

1. **`solutions/`** – Top-level directory containing subfolders for each platform (e.g., `leetcode/` and `work@tech/`).
2. Inside each platform folder, you will find:
   - **Difficulty** subfolders (e.g., `easy/`, `medium/`, `hard/`).
   - Within each difficulty folder, a subfolder for every problem:
     - A solution file in any language (`.py`, `.cpp`, `.js`, `.java`, etc.).
     - A test file (if applicable).
     - A `README.md` with a short problem description and a breakdown of the approach.

## File Naming Convention

To keep things consistent across platforms and languages, each solution follows this pattern:

- **Solution File**:  
  ```
  <platform>-<problem-id-or-name>-<difficulty>.<extension>
  ```
  Examples:
  - `leetcode-1-two-sum-easy.py`
  - `work@tech-123-sample-problem-medium.cpp`

- **Test File** (if you separate tests from the solution):
  ```
  test_<platform>-<problem-id-or-name>-<difficulty>.<extension>
  ```
  Examples:
  - `test_leetcode-1-two-sum-easy.py`
  - `test_work@tech-123-sample-problem-medium.cpp`

- **Problem Description (README)**:  
  A `README.md` located in the same folder as the solution and test files. This contains:
  - A brief problem statement (or a link to the original problem page).
  - An overview of the solution approach (e.g., time complexity, data structures used).

## How to Use

1. **Clone** this repository:
   ```bash
   git clone https://github.com/<your-username>/coding-challenge-solutions.git
   ```
2. **Navigate** to the desired platform (e.g., `leetcode/` or `work@tech/`) and difficulty folder (`easy/`, `medium/`, or `hard/`).
3. **Open** the specific problem folder to see:
   - The **solution** file in your language of choice.
   - The **test** file (if present).
   - The **README** with the problem statement and approach.
4. **Run** the solution using the appropriate tool/command for your chosen language.

## Table of Contents

- [LeetCode](#leetcode)
  - [Easy](#easy)
  - [Medium](#medium)
  - [Hard](#hard)
- [Work@Tech](#worktech)
  - [Easy](#easy-1)
  - [Medium](#medium-1)
  - [Hard](#hard-1)

### LeetCode
#### Easy
- *(List of LeetCode Easy problems...)*

#### Medium
- *(List of LeetCode Medium problems...)*

#### Hard
- *(List of LeetCode Hard problems...)*

### Work@Tech
#### Easy
- *(List of Work@Tech Easy problems...)*

#### Medium
- *(List of Work@Tech Medium problems...)*

#### Hard
- *(List of Work@Tech Hard problems...)*

## Adding a New Problem (PowerShell Example)

Below is a **PowerShell** script snippet for automatically creating a new problem directory and files. Adjust as needed for Bash, Batch, or your preference.

```powershell
# Example: Adding an "easy" problem to LeetCode
# Customize <problem-id-or-name> and <extension> (py, cpp, js, etc.)

# 1. Create the directory
New-Item -ItemType Directory -Path solutions\leetcode\easy\<problem-id-or-name>

# 2. Create the solution file
New-Item -ItemType File -Path solutions\leetcode\easy\<problem-id-or-name>\leetcode-<problem-id-or-name>-easy.<extension>

# 3. Create a corresponding test file (if you maintain separate tests)
New-Item -ItemType File -Path solutions\leetcode\easy\<problem-id-or-name>\test_leetcode-<problem-id-or-name>-easy.<extension>

# 4. Copy the README template
Copy-Item -Path README_TEMPLATE.md -Destination solutions\leetcode\easy\<problem-id-or-name>\README.md
```

Repeat the same process for **Work@Tech** or any other platform by changing the folder path and file naming accordingly.

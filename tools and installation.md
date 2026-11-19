# **Tools and Installation**

Class 1: Tools and Installation | Based on the uploaded transcript

## **1. Industry expectations and AI-assisted development**

The instructor explains how software development expectations are changing.

Earlier:

- Teams received tasks and divided them into sprints.
- A project could take several months to complete.
- Developers frequently depended on colleagues to resolve technical issues.

Current expectations:

- Complete tasks faster and improve productivity.
- Use LLMs as engineering assistants.
- Independently investigate and resolve technical problems.

The instructor discusses using:

- ChatGPT
- Google Gemini
- Claude
- Other emerging LLMs

**Recommended approach:**

- Try solving coding and installation problems using LLMs first.
- Ask instructors when you have doubts about concepts.
- Experiment with different LLMs instead of depending on one model.
- Develop the ability to investigate, debug and solve problems independently.

The instructor recommends a hybrid approach: approximately 90% self-resolution using AI tools and 10% instructor assistance as an example discussed in class.&#x20;

tools and installation(1).txt



## **2. Operating system and CLI**

An operating system (OS) manages different tasks running on a computer.

Examples:

- Opening software.
- Running servers.
- Displaying the user interface.
- Running browsers.
- Managing CPU and RAM resources.

There are two ways to interact with an operating system:

| Interface | Description                                                    |
| --------- | -------------------------------------------------------------- |
| GUI       | Graphical User Interface – windows, icons and menus            |
| CLI       | Command Line Interface – executing commands through a terminal |

Examples of terminals:

| Operating system | Terminal                   |
| ---------------- | -------------------------- |
| Windows          | Command Prompt, PowerShell |
| macOS            | Terminal, Bash             |
| Linux            | Terminal, Bash             |

**Why learn CLI?**

In real-world development, you frequently interact with remote servers that do not have a graphical interface. You need terminal commands to manage files, execute programs and interact with the operating system.&#x20;

tools and installation(1).txt



## **3. Servers**

The instructor introduces servers as powerful computers used to process information and run applications.

Important characteristics:

- Servers have an operating system.
- Linux is commonly used.
- Servers often operate without a graphical user interface.
- Developers connect to servers using terminals.
- Commands are required to interact with them.

This is why CLI knowledge is important for AI engineering and software development.

## **4. Development tools**

The class introduces three important tools:

[File:Visual Studio Code 1.35 icon.svg - Wikimedia Commons](https://images.openai.com/static-rsc-4/YtvW6gSsaaKmwKmq8Vo1tk3qeDR6Xb1HvO4_e6WPOpSp7Oc7z-QKcYvSsaT3xqxrL8ZoopOlKuazuTVar-747xLHihVWojtI1W4tC9qkRTjsNdfmwdPKNmPJ-F0YNK7sn80tabQ0IeblCGrix8hcAGra9EbjFf9Wev5ZGoXcDL0?purpose=inline)

**1. VS Code**

Used to write, edit and debug code. Supports multiple programming languages and extensions.

[TryHackMe | Windows Command Line](https://images.openai.com/static-rsc-4/9UfwfBLG2YldZjGPlwZscSZjoiuKKVDummO4uNwNTInMtM-K5SgaBZno6P1WhuGzkYu8gv8xR_RjOQCBrkNctlHH7VYnvPYfg0R32clSfnr-zt_oDvqfULXEVp1xomVrSeedMKyOhCTEXQZgqKhPEdJwwWvYUnDvXNdjFOxkPEo?purpose=inline)

**2. Terminal / CLI**

Used to execute Python programs, navigate directories, create files and run commands.

[How to publish Python packages to PyPI with GitHub Actions and uv | Nipun Chamikara Weerasiri posted on the topic | LinkedIn](https://images.openai.com/static-rsc-4/P8b5qT6LjdMC6o1iOw8rbxMpEb2slLRuw2bNTusTqb_1OrSyFGckpJmwe44WuRKt13pXSpCZlJIYFz0Ey41Uqq4bAu2oSYfKTqG5ngmHwBEp1M33GdirN4N4oxMZF2-lghDfjmasgUbPJ2Ubof4Gg7E3c8iks8YsFSXRiAQ_qFE?purpose=inline)

**3. UV**

Used to manage Python versions, virtual environments and project dependencies.

### **Editor vs IDE**

| Feature                    | Basic editor | VS Code (hybrid IDE) |
| -------------------------- | ------------ | -------------------- |
| Write code                 | Yes          | Yes                  |
| Syntax highlighting        | Limited      | Yes                  |
| Debugging                  | Limited      | Yes                  |
| Integrated terminal        | No           | Yes                  |
| Multiple files and folders | Limited      | Yes                  |
| Extensions                 | Limited      | Yes                  |

The instructor describes VS Code as a hybrid IDE because it combines editor functionality, terminal access, debugging and extensions.

PyCharm is discussed as a full Python IDE. The instructor prefers VS Code because it is lightweight and supports multiple programming languages.&#x20;

tools and installation(1).txt



## **5. Python installation options**

The instructor explains three approaches.

| Option               | Purpose                                        | Explanation                                        |
| -------------------- | ---------------------------------------------- | -------------------------------------------------- |
| Python.org           | Install Python directly                        | Suitable when you need a particular Python version |
| Anaconda / Miniconda | Python and data science environment management | Provides Conda to manage multiple Python versions  |
| UV                   | Python and project environment management      | Lightweight option recommended for this course     |

**Instructor's recommendation: UV**

Reasons:

- Lightweight.
- Supports multiple Python versions.
- Supports multiple project environments.
- Avoids repeatedly uninstalling and reinstalling Python versions.

tools and installation(1).txt

tools and installation(1).txt

## **6. Why multiple Python versions are required**

The instructor gives an example involving two teams.

- Team A maintains an older application that requires Python 3.4.
- Team B develops a newer Agentic AI application using Python 3.12.

If you install only one Python version globally, switching between these projects becomes difficult.

UV helps manage separate Python environments.

**Example project structure**

**Project A**

Python 3.4 – Environment A

**Project B**

Python 3.12 – Environment B

Illustrative example from the instructor's explanation.

You can switch between environments without uninstalling and reinstalling Python.&#x20;

tools and installation(1).txt



## **7. Global vs local virtual environments**

This is one of the most important concepts in the class.

| Local environment                           | Global environment                              |
| ------------------------------------------- | ----------------------------------------------- |
| Created inside a project folder             | Created in a separate location                  |
| Associated with a particular project        | Can be reused by multiple projects              |
| Keeps project environments separate         | Avoids creating duplicate environments          |
| Useful for isolated application development | Useful for development across multiple projects |

### **Local environment example**

```
Project-A/
    .venv/
    app.py

Project-B/
    .venv/
    app.py
```

Each project maintains its own Python environment.

### **Global environment example**

```
Python Environments/
    Environment-A/
    Environment-B/

Project-A/
    app.py

Project-B/
    app.py

Project-C/
    app.py
```

Projects can select a shared global environment when the Python version and dependencies are suitable.

**Instructor's guidance:**

- Global environments are useful when experimenting or working across multiple projects.
- Local environments are recommended for isolated project development and final deployment.
- The instructor emphasizes local environments for production applications.&#x20;

  tools and installation(1).txt



## **8. Terminal commands covered**

The instructor introduces basic commands for navigating and managing files.

| Command            | Purpose                                    |
| ------------------ | ------------------------------------------ |
| `cd foldername`    | Enter a directory                          |
| `cd ..`            | Move to the parent directory               |
| `dir`              | List files and folders in Windows CMD      |
| `ls`               | List files and folders in Unix/Linux/macOS |
| `ls -la`           | List files, including hidden files         |
| `mkdir foldername` | Create a directory                         |
| `rmdir foldername` | Remove an empty directory                  |

Example:

```
cd assignment
cd ..
dir
mkdir myproject
rmdir myproject
```

The instructor also demonstrates creating files through the command line.

tools and installation(1).txt

## **9. Installation instructions discussed**

The installation sequence covered in the transcript is:

1. Install UV.
2. Install VS Code.
3. Open VS Code.
4. Open the project folder.
5. Open the integrated terminal.
6. Select Command Prompt or PowerShell.
7. Practice the terminal commands.
8. Start working with UV environments.

For Windows:

- The instructor generally recommends Command Prompt.
- PowerShell is used when installation instructions specifically require it.
- UV installation instructions are taken from the official Astral documentation.

The instructor also mentions that installation commands, software links and reference files will be shared in a ZIP file.&#x20;

tools and installation(1).txt

tools and installation(1).txt



## **10. Assignments and practice**

The instructor specifically mentions these learning expectations:

- Watch the prerequisite Python classes.
- Practice the OS Command Cheat Sheet.
- Learn Windows CMD and Unix commands.
- Install and become familiar with VS Code.
- Install UV.
- Practice creating and switching Python environments.
- Use LLMs to investigate installation and coding errors.

The instructor gives students five additional days to practice and complete the work.

## **Important concepts to remember**

| Topic              | What you should remember                                    |
| ------------------ | ----------------------------------------------------------- |
| LLMs               | Use AI tools to investigate and resolve technical issues    |
| CLI                | Interact with the OS using commands                         |
| Server             | A computer used to process information and run applications |
| VS Code            | Editor, debugger and integrated development environment     |
| UV                 | Manage Python versions and environments                     |
| Python versions    | Different projects may require different versions           |
| Local environment  | Environment inside a project                                |
| Global environment | Environment reusable across projects                        |
| Production         | Keep the application's environment isolated                 |

## **Practice checklist**

**Class 1 preparation**

0/10 completed

Watch prerequisite Python classes

Install VS Code

Install UV

Open VS Code integrated terminal

Practice cd, cd .., dir and ls

Create and delete folders using CLI

Understand Python.org vs Conda vs UV

Create separate local virtual environments

Understand global vs local environments

Practice switching between Python versions

**My recommendation for revision:** Give extra attention to CLI commands, UV installation, and global vs local environments. These are the main practical concepts emphasized in this transcript.

*Note: This summary covers the uploaded transcript, which ends during the explanation of global and local environments. It does not establish that Jupyter Notebook or RAG was covered in this particular class.*


# **Summary – AI Forward Deployed Engineering Bootcamp**

**Session: Tools and Installation (Part 2)**

This transcript continues the earlier tools-and-installation session. It mainly covers **UV virtual environments, running Python files, Jupyter notebooks in VS Code, Google Colab, and how to practise Python for the upcoming bootcamp classes.**

## **1. Main topics covered**

Covered

**UV – Python environment management**

- Creating local and global virtual environments.
- Installing specific Python versions.
- Activating environments.
- Running Python programs using the activated environment.

  Covered

  **Jupyter Notebook in VS Code**
- Creating `.ipynb` files.
- Installing the Jupyter extension.
- Selecting Python kernels.
- Running individual cells and writing Markdown.

  Covered

  **Google Colab**
- Running Python in a browser.
- Creating notebooks.
- Using hosted runtime resources.
- Using GPU resources for experiments.

  Covered

  **Python practice and course expectations**
- Practising Python independently.
- Using LLMs to troubleshoot errors.
- Understanding when to use local VS Code or Google Colab.

## **2. UV virtual environments**

UV is a software tool used to manage Python versions and virtual environments.

A virtual environment provides an isolated Python installation and its libraries.

### **A. Local virtual environment**

A local environment is created inside the project directory.

Example:

```
Project-A/
    .venv/
    main.py
```

The instructor demonstrates creating an environment with Python 3.12:

```
uv venv --python 3.12
```

**Windows activation:**

```
.venv\Scripts\activate
```

**macOS/Linux activation:**

```
source .venv/bin/activate
```

Verify the Python version:

```
python --version
```

Run a Python program:

```
python temp1.py
```

Exit the Python interactive interpreter:

```
exit()
```

**Important:** Once activated, the terminal uses the Python executable from that environment. The project folder itself does not activate or select Python; the terminal's active environment determines which Python is used.

### **B. Global virtual environment**

A global environment is stored in a central directory rather than inside an individual project.

Example:

```
D:\PythonEnvironments\
    uvfd1\
    python312\
    python310\
```

Create a central directory first, then specify its path when creating an environment:

```
uv venv --python 3.12 D:\PythonEnvironments\uvfd1
```

The activation path will point to the central environment:

```
D:\PythonEnvironments\uvfd1\Scripts\activate
```

On macOS/Linux, the activation script is under `bin` instead of `Scripts`.

### **C. Local vs global environments**

| Feature      | Local                    | Global                          |
| ------------ | ------------------------ | ------------------------------- |
| Location     | Inside project           | Central directory               |
| Reusability  | Project-specific         | Can be reused across projects   |
| Organization | Each project has its own | Centralized                     |
| Best use     | Project isolation        | Development and experimentation |

The instructor prefers global environments during development and experimentation, while emphasizing project-specific isolation for final projects and deployment-related work.

The important distinction is that a global environment is also a virtual environment. It is not the same as installing Python globally for the entire operating system.&#x20;

tools and installation(1).txt



## **3. Running Python programs**

The instructor demonstrates running a Python file from the terminal.

Example:

```
Project/
    temp1.py
```

Check whether the file exists:

```
dir
```

Run it:

```
python temp1.py
```

The Python executable comes from the currently activated environment.

You can use either an absolute file path or a relative file path to run the program.

**Key takeaway:** You should understand which Python environment your terminal is using before executing a program.

## **4. Python&#x20;**`.py`**&#x20;vs&#x20;**`.ipynb`

One important part of the session is understanding the difference between Python files and Jupyter notebooks.

| Feature         | `.py`                            | `.ipynb`                     |
| --------------- | -------------------------------- | ---------------------------- |
| File type       | Python script                    | Jupyter Notebook             |
| Execution       | Usually runs the complete script | Runs individual cells        |
| Experimentation | Less interactive                 | Highly interactive           |
| Markdown notes  | Separate documentation           | Supported inside notebook    |
| Common use      | Application code                 | Learning and experimentation |

### **Why use Jupyter Notebook?**

Suppose you have 100 lines of Python code.

In a `.py` file, you generally execute the script.

In a notebook, you can execute only the cell you want.

For example:

```
# Cell 1a = 10b = 20print(a + b)
```

```
# Cell 2name = "Python"print(name)
```

You can execute these cells independently, examine the output, change the code, and experiment.

You can also add Markdown cells to document your learning.

The instructor explains that notebooks are useful for AI engineers and data scientists when experimenting with code. Once the code is finalized, it can be moved into a normal `.py` file for application development.&#x20;

tools and installation(2).txt



## **5. Configure Jupyter in VS Code**

The instructor demonstrates the following setup.

1. **Create a notebook**

   Create a file with the `.ipynb` extension in VS Code.
2. **Install the Jupyter extension**

   Open VS Code Extensions, search for `Jupyter`, and install it.
3. **Select the Python kernel**

   Open the notebook and select:

   `Select Kernel → Python Environments`
4. **Choose the Python environment**

   Select the environment that you want to use to execute notebook cells.
5. **Run notebook cells**

   Use the Run or Execute Cell button and inspect the output.

### **What is a kernel?**

A kernel is the running execution environment that executes notebook code.

For example, you might have:

- Local Python 3.10 environment.
- Global Python 3.12 environment.

You can select the appropriate Python environment as the notebook kernel.

### **Problem: VS Code cannot detect the global environment**

The instructor demonstrates an issue where VS Code detects a local environment but cannot automatically find a global environment stored outside the current project directory.

The solution demonstrated:

1. Activate the global environment.
2. Install `ipykernel` in that environment.
3. Register the environment as a Jupyter kernel.
4. Give the kernel a display name.
5. Restart VS Code.
6. Select the newly registered kernel.

The instructor also explains that the kernel registration tells VS Code where to find the Python environment.

tools and installation(2).txt

## **6. Google Colab**

[Getting Started with Google Colab: A Beginner's Guide](https://images.openai.com/static-rsc-4/2H77lb545U9VInHrH9yWjILf2-G6yANS_Kkp3kcz8UnDziAERMWPaTchA57F4gNZ0lYRX9PnSlD1sPxaH29c2sF5ZIGNyt4tZFD6zsa642-8lrGMPcyp9S_xJh_TJXAuLs0-sYw4xjjfrRsVEnftG0hgCGAetS7zBjoVsg6cAqA?purpose=inline)

[Google Colab](https://images.openai.com/static-rsc-4/M2nWKN-Rlho7nfQH-MSAhXfyMBTPemt_nAVO-TbrBDOZxsuKNwA99gYdmndoDqMEjKkqv8N6X893owdtHBVN143NaJ5njgd8p3HOYa6kCy9pfNYAyUQ8-dr3C4wLnN4qyxekoqrt8biHvR4WjwRkcogUxUYA-1Vpk4F1FXSkoMI?purpose=inline)

[無料＆簡単！Google ColabでPython入門する最短ルート｜しろくま@Python/AI/データ分析](https://images.openai.com/static-rsc-4/8Z4NAAgprplvUvno0jv8PzvZfHKdUWbdjvI3OfblAH5puHRUP_sO3WspijZ3u7aHuZljFRSVYavLUInN0XK8v3_5wiI66bxyjvJGq1pePeb3wo2cNuSXBdcWyahoLaYru9R6QLzrjXWsT1fOMGWnoszE7w2Ojj14FX2GnAzFino?purpose=inline)

4

Google Colab is introduced as an alternative for people who face difficulties installing Python or UV locally.

It allows you to execute Python notebooks through a browser.

### **How to start**

1. Open Google Colab.
2. Sign in using your Google account.
3. Select New Notebook.
4. Write Python code inside a cell.
5. Click Run.
6. Google connects the notebook to a hosted runtime.

Example:

```
print("Hello AI Engineering")
```

Check the Python version:

```
import platformprint(platform.python_version())
```

### **Features demonstrated**

- Run Python code in browser.
- Execute individual notebook cells.
- Write Markdown.
- Use hosted RAM and disk resources.
- Access GPU runtime options.
- Use a terminal within the Colab environment.

The instructor demonstrates a hosted environment with approximately 12.7 GB RAM and 107 GB disk at that time. These figures are specific to the demonstration, not guaranteed Colab specifications.

### **Important limitation**

When the Colab runtime disconnects or is restarted, runtime memory and temporary execution state are lost. Save important work and files appropriately.

tools and installation.txt

## **7. VS Code + UV vs Google Colab**

During the discussion, a student asks which environment is recommended.

The instructor explains that both are useful, depending on the work.

| Scenario                                                    | Recommended environment                           |
| ----------------------------------------------------------- | ------------------------------------------------- |
| Normal Python development                                   | VS Code + UV                                      |
| Python application development                              | VS Code + UV                                      |
| Learning and experimenting                                  | Jupyter Notebook                                  |
| Running experiments with GPU requirements                   | Google Colab                                      |
| Testing open-source LLMs that need more computing resources | Google Colab, if suitable resources are available |

**Practical understanding:**

- Use VS Code + UV for local development and project organization.
- Use Google Colab when your computer does not have sufficient computing resources for an experiment.
- Both VS Code notebooks and Colab use the `.ipynb` file format.

tools and installation.txt

## **8. Additional concepts discussed**

### **Terminal inside VS Code**

The instructor clarifies that UV commands are executed in a terminal, not directly inside the VS Code editor.

VS Code simply provides an integrated terminal, so you do not need to switch applications.

UV can also be used from a separate operating-system terminal.

### **Useful commands**

| Command            | Purpose                      |
| ------------------ | ---------------------------- |
| `dir`              | List files on Windows        |
| `ls`               | List files on macOS/Linux    |
| `ls -la`           | Show detailed file listing   |
| `cls`              | Clear Windows terminal       |
| `clear`            | Clear macOS/Linux terminal   |
| `python --version` | Check Python version         |
| `python temp1.py`  | Execute Python file          |
| `exit()`           | Exit Python interactive mode |

### **Downloading notebooks**

The instructor also demonstrates downloading a notebook from Google Colab and opening the same `.ipynb` file in VS Code.

This shows that notebook files can be moved between these environments.&#x20;

tools and installation(2).txt



## **9. Course expectations and learning guidance**

The instructor emphasizes:

1. Complete the prerequisite Python lessons.
2. Practise the commands demonstrated during the session.
3. Learn how to troubleshoot installation problems independently.
4. Use LLMs to investigate errors and understand solutions.
5. Do not depend entirely on the instructor for coding practice.
6. Spend at least one hour daily practising programming, as recommended during the closing discussion.
7. The initial two or three classes will refresh Python concepts before moving further into the bootcamp syllabus.

The instructor also mentions that assignments are for individual learning and do not need to be submitted.&#x20;

tools and installation(2).txt

tools and installation(2).txt



## **10. Practical checklist – what you should complete**

Use this checklist to track your progress.

**Installation practice tracker**

0/13 completed

Install UV and verify that it works in a new terminal.

Create a local Python 3.12 virtual environment.

Activate the local environment and check the Python version.

Create a central directory for global environments.

Create and activate a global virtual environment.

Create a temp1.py file and execute it.

Install the Jupyter extension in VS Code.

Create a .ipynb notebook and execute multiple cells.

Select different Python kernels.

Register a global environment as a Jupyter kernel.

Create a Google Colab notebook.

Execute Python code and check the runtime Python version.

Download a Colab notebook and open it in VS Code.

Reset checklist

## **11. Most important things to remember**

For revision, focus on these five concepts:

1. **UV:** Manages Python versions and virtual environments.
2. **Local vs Global:** Understand where environments are stored and when they can be reused.
3. **Python&#x20;**`.py`**:** Used for normal Python scripts and application code.
4. **Jupyter&#x20;**`.ipynb`**:** Used for interactive development, experiments and learning.
5. **Google Colab:** Useful for browser-based Python execution and experiments requiring additional computing resources.

**My recommendation for revision:** Practise creating and activating environments first. Then spend time with Jupyter notebooks and Google Colab. These are the foundational tools demonstrated in this session.

The transcript also mentions Python package management (pip/PyPI) as a topic to be explained, but this section does not provide a complete lesson on it.

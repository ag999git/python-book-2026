

## VS Code

### Table of Contents
- [1. VS Code Basics](#1-vs-code-basics)
- [2. Setup](#2-setup)
- [3. VS Code Interface](#3-vs-code-interface)
- [4. Some important Extensions for Python programming](#4-some-important-extensions-for-python-programming)
- [5. Python workflow in VS Code](#5-python-workflow-in-vs-code)
- [6. How to Create a Python Project](#6-how-to-create-a-python-project)
- []()
- []()


### 1 VS Code Basics

### 1.1 VS Code Introduction
VS Code is best described as A local desktop IDE/editor. It can run on Windows/Mac/Linux.

### 1.2 Downloading VS Code (Step-by-step)
#### 1.2.1 Step 1: Go to the official website
    

Open your browser (Chrome/Edge) and type:    
[https://code.visualstudio.com/](https://code.visualstudio.com/)
    
#### 1.2.2 Step 2: Choose your operating system    
For Windows OS: ➡ Click "Download for Windows"
    
A file named something like:- VSCodeUserSetup-x64-1.xx.x.exe will start downloading.
    
#### 1.2.3 Step 3: Wait for download to complete
    
You will see the .exe file in your Downloads folder.
    
### 1.3 Installing VS Code (Step-by-step)
    
#### 1.3.1 Step 1: Double-click the installer
    
Open your Downloads folder → Double-click the file:
    
VSCodeUserSetup-x64-...
    
#### 1.3.2 Step 2: License Agreement
    
Click “I accept the agreement” → Next.
    
#### 1.3.3 Step 3: Choose installation location
 
    
Beginners should leave it as:-
    
C:\\Users\\<YourName>\\AppData\\Local\\Programs\\Microsoft VS Code
    
Click Next.
    
#### 1.3.4 Step 4: Additional tasks — VERY IMPORTANT
    
You will see checkboxes.
    
Tick these:
    
✔ Add "Open with Code" to File Explorer  
✔ Add "Open with Code" to Folder context menu  
✔ Register Code as editor for supported file types  
✔ Add to PATH (very important for Python users)
    
Click Next.
    
#### 1.3.5 Step 5: Install
    
Click Install and wait.
    
#### 1.3.6 Step 6: Launch

Tick "Launch Visual Studio Code" → Finish.


### 2 Setup

### 2.1 First-time Setup
When VS Code launches:
    
#### 2.1.1 You may see:
    
*   “Do you trust this author?” → Click **Yes**
*   “Would you like to install recommended extensions?” → Optional
  VS Code opens with a **welcome page** that includes:
    *   A "Get Started" guide
    *   Themes (light/dark)
    *   Buttons to create/open files
    
### 3 VS Code Interface

![UI](https://github.com/ag999git/python-book-2026/blob/main/chapter-1-Python-Basics-I/vs-code-images/VS-code-main-parts-of-UI.jpg)

#### 3.1 Main parts of the UI of VS Code
    
Below is the simplest explanation of each part:
    
#### 3.2 A. Activity Bar (left side icons)
    
This vertical bar has 5–6 icons. The **Activity Bar** is the thin bar on the far left that lets you switch between different views within the **Side Bar**. The icons typically found here (from top to bottom) are:-

![Activity Bar (left side icons)](https://github.com/ag999git/python-book-2026/blob/main/chapter-1-Python-Basics-I/vs-code-images/VS-code-activity-bar.jpg)



#### 3.3 B. Sidebar (shows details)
    

The **Side Bar** displays the content of the view currently selected in the **Activity Bar** (e.g., the File Explorer, Search results, etc.). The icons and buttons within the Side Bar change based on the selected view:
    
Each one of the Sidebar views are discussed as follows:-
    
#### 3.4  When you click 📁 Explorer, you will see:
#

*   Your opened folder
*   Files inside it
    Ueful for Python beginners:  
    ✔ Create new files  
    ✔ Create folders  
    ✔ See your project structure
    
    | Icon | Name | Function |
    | --- | --- | --- |
    | New File (Sheet of paper with a plus) | New File | Creates a new file in the currently selected folder. |
    | New Folder (Folder with a plus) | New Folder | Creates a new folder in the currently selected folder. |
    | Refresh Explorer (Circular arrows) | Refresh | Reloads the file list to reflect changes made outside VS Code. |
    | Collapse All (Two triangles pointing left) | Collapse All | Collapses all expanded folders in the Explorer tree. |
    | Open Editors (Icon with lines) | Open Editors | Toggles the section showing all currently open files. |
    
    #### 3.5      Search View Icons (Top Toolbar)
    
    # 
    
    | Icon | Name | Function |
    | --- | --- | --- |
    | Match Case (Uppercase 'Aa') | Match Case | Makes the search case-sensitive. |
    | Match Whole Word (Square box with lines) | Match Whole Word | Only matches the full word entered in the search box. |
    | Use Regular Expression (.*) | RegEx | Enables Regular Expression syntax for searching. |
    | Replace (Left-pointing arrow) | Replace | Toggles the Replace input box. |
    
    #### 3.6      Editor Group (Center)
    
    # 
    
    This is the primary area where you view and edit your code. It consists of one or more open file tabs and various controls. You can open multiple files as tabs (like browser tabs):
    
    | Icon | State | Meaning |
    | --- | --- | --- |
    | Dot or Circle on the tab | Dirty/Unsaved | The file has been modified but not yet saved. |
    | Cross/X on the tab | Close | Closes the open file. |
    | Split Editor (Two vertical boxes) | Split Editor | Splits the current editor to view files side-by-side. |
    | More Actions (Three dots) | More Actions | Opens a menu with additional commands for the editor group. |
    
    #### 3.7      Panel (Bottom)
    
    # 
    
    The **Panel** appears at the bottom of the window and can contain several views. You switch between them using tabs.
    
    | Tab Name | Function |
    | --- | --- |
    | Terminal | An integrated command-line interface for running shell commands. |
    | Output | Shows output from tasks, build systems, or extensions. |
    | Problems | Lists compilation errors, warnings, and linter issues in your project. |
    | Debug Console | Allows you to interact with the debugging session, evaluate expressions, and view log messages. |
    
    #### 3.8      Status Bar (bottom blue bar)
    
    # 
    
    The **Status Bar** sits at the very bottom and displays contextual information about the open file and project, often with clickable actions.
    
    | Example Icon/Text | Name | Function |
    | --- | --- | --- |
    | Branch Name (e.g., main with a branch icon) | Git Branch | Shows the current Git branch. Clicking allows you to switch or create new branches. |
    | Error/Warning Counts (e.g., 1 Error, 3 Warnings) | Problems Status | Shows the count of problems; clicking opens the Problems Panel. |
    | Language Mode (e.g., Plain Text, JavaScript) | Language Mode | Displays the language of the active editor. Clicking lets you change it. |
    | Indentation (e.g., Spaces: 4) | Indentation Settings | Shows the tab size and whether tabs or spaces are used. Clicking lets you change the settings. |
    | Line/Column (e.g., Ln 10, Col 25) | Cursor Position | Shows the current line and column number of the cursor. |
    | Manage/Gear Icon (Far right) | Manage | Another quick access to settings and themes (can also be found in the Activity Bar). |
    
    If you install Python, VS Code detects it.
   
      
    
### 4 Some important Extensions for Python programming
    
# 
    
Open **Extensions** → search → install:
    
##### 4.1 Python (Microsoft)  
Python highlighting  
Runs scripts  
Jupyter notebook support  
Autocomplete
    
#### 4.2 Pylance  
Better IntelliSense
    
#### 4.3 Jupyter  
Lets you run .ipynb notebooks inside VS Code
    
#### 4.4 Code Runner (optional)  
Run code with one click

 

### 5 Python workflow in VS Code

#### A Beginner’s VS Code + Python Workflow (Step-by-Step)

This is the simplest workflow for complete beginners.


#### 5.1 Step 1: Install Python

Download from:- https://www.python.org/downloads/

During installation, tick this box:

✔ **Add Python to PATH** (very important)

#### 5.2 Step 2: Install VS Code


(You already have the installation steps earlier.)

#### 5.3 Step 3: Install Python extension in VS Code


*   Open VS Code → Left toolbar → Extensions icon (square) →

*   Search for Python
*   Install the official Microsoft extension.

#### 5.4 Step 4: Create a folder for your project


For example:

`D:\\Python\_Projects\\MyFirstProject`

This folder will hold _all_ your code files.


#### 5.5 Step 5: Open the folder in VS Code


VS Code → **File → Open Folder** → Select your folder.

This is important because VS Code needs a **workspace folder**.


#### 5.6 Step 6: Create a Python file


In Explorer:

➡ Click **New File**  
Name it:- `main.py`

  

#### 5.7 Step 7: Write your code


Example:

`print("Hello World!")`


#### 5.8 Step 8: Open the VS Code Terminal

Shortcut:

~~~
Ctrl + `
~~~

This opens a terminal panel at the bottom.


#### 5.9 Step 9: Run your Python script


Type:- `python main.py`

Press Enter.

You will see:

`Hello World!`


That’s it — you completed the basic workflow!

  
### 6. How to Create a Python Project

Here are the recommended steps for beginners.

#### 6.1 Step 1: Create a folder



Example:

`C:\Python\My_App`

#### 6.2 Step 2: Add subfolders (optional but good practice)

```python
My_App/  
    ├── main.py
    ├── helper\_functions.py    
    └── data/
```

Note that every project having multiple files has to have an entry point. By convention, though not required, the entry point is often named main.py. Why Do We Use It?

1.                 The name `main.py` serves a clear purpose for both humans and tools.

2.                 Identifies the Entry Point: It immediately signals to anyone reading the project (another developer, a user, or even your future self) that this file contains the primary execution logic.

3.                 Facilitates Command Line Execution: When you run a project from the command line, you must specify which file to execute. Using a consistent name like main.py makes running the application straightforward: python main.py.

4.                 Project Structure and Packaging: When you package a complex Python application or library (e.g., using setuptools), you often need to define an "entry point" script. Naming your core script main.py keeps the internal project logic clean and predictable.

#### 6.3 Step 3: Open the folder in VS Code


`File → Open Folder → Select My_App`

#### 6.4 Step 4: Add Python files


Examples:

*  ` main.py` → main program
*   `helper_functions.py` → reusable functions
*   `config.py` → any settings

#### 6.5 Step 5: Install required libraries (optional)


`Terminal → run:`

`pip install requests`

`pip install numpy`



### 7 How to Run Python Scripts in VS Code**

There are **3 beginner methods**:

#### 7.1 Method 1: Using Terminal (most recommended)

Open terminal:

~~~python
Ctrl + `

~~~

Run:

`python main.py`

✔ Works always  
✔ Most reliable  
✔ Teaches real-world workflow

#### 7.2 Method 2: Using the Run Button (triangle icon)

In a Python file, VS Code may show a **Run Python File** button on top.

Click it → Output appears in **TERMINAL**.

  

#### 7.3 Method 3: Using Code Runner Extension (optional)

Install **Code Runner** → A ▶ icon appears.

Run code with one click.

Not recommended for advanced use, but beginners like it.


  
### 8 Common Beginner Errors + Quick Fixes

These are the most common problems Indian beginners face on Windows.
 

#### 8.1 ERROR 1: "python is not recognized"

**Cause:** Python was not added to PATH.

**Fix:-** Option A — Reinstall Python → select:

Fix:- Option B:- **Add Python to PATH**

To do so manually:
  
2.  Search "Edit system environment variables"
  
4.  Click **Environment Variables**
  
6.  Under **Path**, add:

`C:\Users\<YourName>\AppData\Local\Programs\Python\Python3x\`

and

`C:\Users\<YourName>\AppData\Local\Programs\Python\Python3x\Scripts\`


  

#### 8.2 ERROR 2: VS Code shows "Select Python Interpreter"

**Fix:-** Bottom-left → click where it says: Python: <version>. Pick correct interpreter:

Example:

`Python 3.12.0  (C:\Users\YourName\AppData\...)`

#### 8.3 ERROR 3: 'pip' not working

Run:

`python -m pip install <package>`

  

Example:

`python -m pip install requests`

  

#### 8.4 ERROR 4: Running the wrong file

Beginners often write code in one file but run another.

**Fix:-** Always run:

`python <your current file>.py`

#### 8.5 ERROR 5: VS Code Terminal opens PowerShell

Sometimes PowerShell causes execution issues.

**Fix (switch to Command Prompt):**

`VS Code → Terminal → New Terminal → click dropdown → select: Command Prompt`

#### 8.6 ERROR 6: Accidentally created a workspace file (.code-workspace)

Harmless. Just close and reopen folder.

#### 8.7 ERROR 7: File saved with wrong extension

Beginners sometimes do:- `main.py.txt`

**Fix:-** Save as:

`main.py`





### test

### 9 Debug

#### 9.1 Debugging Python Code in VS Code (Beginner Guide)**

Debugging means:  
✔ finding mistakes  
✔ stopping the program at certain points  
✔ checking variable values  
✔ running line-by-line

#### 9.2 Make sure Python extension is installed

Left toolbar → Extensions → search for Python

Install the **Microsoft Python extension**.

#### 9.2 Create a small sample file to debug

Example file:- `debug_example.py`

```python
def add(x, y):
    result = x + y
    return result
a = 10
b = 5
total = add(a, b)
print("The total is:->", total)


```

#### 9.3 Set a BREAKPOINT

A **breakpoint** stops your program temporarily.

How to set:- (a) Click on the **left margin** next to the line number. (b) You will see a **red dot** • (c) Clicking on the red dot adds a breakpoint

#### 9.4 Start debugging

Go to the left toolbar → Click the **Run & Debug icon** (a play button with a bug).

OR press:- F5

##### First time only:

You will see:-Select a debug configuration

Choose:- Python: Current File

#### 9.5 Program stops at the breakpoint

Now the program pauses on the red dot.

You can now inspect everything.

#### 9.6 Debugger Tools You Will See

When stopped at a breakpoint, a debug toolbar appears at the top:

| Button | Meaning |
| --- | --- |
| ▶ Continue | Run normally until next breakpoint |
| ↷ Step Over | Run next line (skip inside functions) |
| ↳ Step Into | Go inside function line-by-line |
| ↺ Step Out | Finish current function and return |

#### 9.7 Watch variable values

When you debug code, sometimes you want to keep an eye on certain variables without constantly printing them or searching for them in the call stack.  
The **Watch** panel lets you do exactly that.

##### 9.7.1 Where they appear

While debugging, open:

View → Run and Debug → WATCH panel (left sidebar)

##### 9.7.2 Inspect Watch Variables

The **Side Bar** in the **Run and Debug** view provides several panels for inspection:

##### 9.7.3 A. Variables

This panel automatically shows the current value of all **Local** variables (variables defined within the current function/scope) and **Global** variables. As you step through the code, these values update in real-time.

##### 9.7.4 B. Watch

The **Watch** panel allows you to explicitly monitor variables or expressions.

1.  Click the **Add Expression** button (usually a + icon) in the **Watch** panel.
2.  Type the name of a **variable** (e.g., my\_list) or a **complex expression** (e.g., len(my\_list) > 5).
3.  The value of the watched variable/expression will be displayed and updated automatically every time the debugger pauses. This is helpful for keeping track of key values across multiple steps.

##### 9.7.5 C. Call Stack

This panel shows the sequence of function calls that led to the current line of execution, which is helpful for understanding program flow.

##### 9.7.6 D. Debug Console

You can execute arbitrary Python commands and evaluate expressions in the **Debug Console** (found in the **Panel** at the bottom) while the code is paused. For example, you can type print(my\_variable) or even change a variable's value directly.

#### 9.8 What you can do with Watch Variables

*   Add a variable name (e.g., count, user.name)
*   Add expressions (e.g., a + b, len(items))
*   VS Code will **update their values live** as you step through the program.

##### 9.8.1 Why Watch Variables are useful

*   Track how a value changes over time
*   Debug logic errors
*   Avoid adding temporary print statements
*   Inspect nested objects or expressions easily

##### 9.8.1 Hover to inspect variables

Simply place your mouse over any variable:

Example:

Hover over a → small popup shows:

`10`

Very useful!

##### 9.8.2 Adding a new breakpoint

You can add multiple breakpoints on different lines.

Example:  
Add one inside the function:

`result = x + y`

Now debugging will stop inside the function too.

##### 9.8.3 ✔ Example Debugging Flow (beginner)

1.  Start debugging (F5)
2.  Execution stops at breakpoint
3.  Hover variables to see values
4.  Click "Step Into" to enter function
5.  Move line by line
6.  Watch how variables change
7.  Click "Continue" to finish

### 10 Debugging common beginner mistakes

#### 10.1 ❌ Error example:-

`print(result)`

But you never defined result.

Debugger will show:

`NameError: name 'result' is not defined`

You can use "Call Stack" + stepping to find where it failed.

#### 10.2 Debugging input() programs

If your script has `input()`:

`name = input("Enter your name: ")`

Debugger will pause and ask for input in terminal.

#### 10.3 Debug Configuration (optional)

VS Code may create a `.vscode/launch.json` file.

Beginners do NOT need to edit it.

Just choose:

Python: Current File

#### 10.3 Summary: VS Code Debug Steps

1.  Open your Python file
2.  Set a breakpoint (red dot)
3.  Press **F5** (Run & Debug)
4.  Program pauses
5.  Inspect variables
6.  Step line-by-line
7.  Fix mistakes






















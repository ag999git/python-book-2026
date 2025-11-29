

## VS Code

### Table of Contents
- [1. VS Code Basics](#1-vs-code-basics)
- [2. Setup](#2-setup)
- [3. VS Code Interface](#3-vs-code-interface)
- [4. Some important Extensions for Python programming](#4-some-important-extensions-for-python-programming)
- [5. Python workflow in VS Code](#5-python-workflow-in-vs-code)
- [6. How to Create a Python Project](#6-how-to-create-a-python-project)
- [7. How to Run Python Scripts in VS Code](#7-how-to-run-python-scripts-in-vs-code)
- [8. Common Beginner Errors and Quick Fixes](#8-common-beginner-errors-and-quick-fixes)
- [9. Debug](#9-debug)
- [10. Debugging common beginner mistakes](#10-debugging-common-beginner-mistakes)
- [11. FAQ](#10-faq)
- [12. FAQ VS Code User Interface](#12-faq-vs-code-user-interface)


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
    
`C:\Users\<YourName>\AppData\Local\Programs\Microsoft VS Code`
    
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

[Back to Table of Contents](#table-of-contents)

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
    
[Back to Table of Contents](#table-of-contents)

### 3 VS Code Interface
[Back to Table of Contents](#table-of-contents)

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
   
      
[Back to Table of Contents](#table-of-contents)

### 4 Some important Extensions for Python programming
    
[Back to Table of Contents](#table-of-contents)

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

 [Back to Table of Contents](#table-of-contents)

### 5 Python workflow in VS Code

[Back to Table of Contents](#table-of-contents)

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

[Back to Table of Contents](#table-of-contents)

  
### 6. How to Create a Python Project

[Back to Table of Contents](#table-of-contents)

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


[Back to Table of Contents](#table-of-contents)


### 7. How to Run Python Scripts in VS Code

[Back to Table of Contents](#table-of-contents)

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


[Back to Table of Contents](#table-of-contents)
  
### 8 Common Beginner Errors and Quick Fixes

[Back to Table of Contents](#table-of-contents)

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




[Back to Table of Contents](#table-of-contents)

### 9 Debug

[Back to Table of Contents](#table-of-contents)

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


[Back to Table of Contents](#table-of-contents)

### 10 Debugging common beginner mistakes

[Back to Table of Contents](#table-of-contents)

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





[Back to Table of Contents](#table-of-contents)



### 11. FAQ
(Frequently Asked Questions)

[Back to Table of Contents](#table-of-contents)

#### 1. What is VS Code?
VS Code (Visual Studio Code) is a free, lightweight code editor made by Microsoft.
It is not a full heavyweight IDE like PyCharm, but it becomes powerful by adding extensions (plugins).

#### 2. Is VS Code free to download?
✅ Yes, 100% free
You can use it forever — no trial, no subscription.

#### 3. Where should I download VS Code from?
Always download from the official Microsoft website:
 https://code.visualstudio.com/
Never download from third-party websites.

#### 4. What version should I download for Windows?
Choose this:- User Installer (64-bit)
This is the simplest and recommended for beginners.

#### 5. How do I install VS Code after downloading?
Steps:
1.	Double-click the downloaded .exe file
2.	Accept the license
3.	Click Next → Next → Install
4.	When installation completes, check Launch VS Code
5.	Click Finish
That’s it!

#### 6. Do I need to install Python before using VS Code?
Yes. VS Code does not include Python.
Download Python from:
 https://www.python.org/downloads/
Make sure you check:
✔ Add Python to PATH (VERY important for Windows)

#### 7. Do I need to add Python to PATH manually?
If you checked Add Python to PATH during installation → No
If not → VS Code will not detect Python.
To fix it:
Reinstall Python → check Add to PATH

#### 8. How do I check if Python is installed correctly?
Open Command Prompt and type:
python --version
If it shows a version like 3.12.x, you're good.
If you see:
‘python’ is not recognized...
→ Python PATH is not set → reinstall Python with PATH enabled.

#### 9. How do I install Python extension in VS Code?
Open VS Code → left sidebar Extensions icon → search:
Python
Click Install on:
✔ Microsoft Python extension (official)
VS Code will now:
•	Detect Python
•	Enable debugging
•	Enable IntelliSense (autocomplete)
•	Show errors and warnings

#### 10. Do I need any other extensions as a beginner?
Not required.
But recommended:
✔ Python (by Microsoft)
✔ Pylance (improves autocomplete)
✔ Jupyter (for Notebook-style code)

#### 11. VS Code says “Python not found”. What should I do?
Try the following:
1.	Close VS Code
2.	Reinstall Python with Add to PATH checked
3.	Reopen VS Code
4.	Press Ctrl + Shift + P → Type:
5.	Python: Select Interpreter
6.	Choose the Python version installed on your PC
This solves most issues.

#### 12. Should I use VS Code or PyCharm as a beginner?
Use VS Code because it is:
•	lighter
•	easier to navigate
•	fast to install
•	works well on normal laptops
•	easier for school/college beginners
PyCharm is very powerful but heavier.

#### 13. Will VS Code slow down my computer?
No.
It is one of the most lightweight code editors.

#### 14. Do I need internet to use VS Code?
Only for installing extensions the first time.
After that, no internet needed for writing or running code.

#### 15. Can I run Python scripts inside VS Code?
Yes.
Just open your .py file and click:
▶ Run
or press:
Ctrl + F5

#### 16. What if I open VS Code and see a blank screen?
You must open a folder, not individual files.
Steps:
1.	Click File → Open Folder
2.	Select your project folder
3.	Now VS Code will detect files properly

#### 17. Is VS Code safe to install in college computers?
Yes, VS Code is from Microsoft and is widely used in:
•	engineering colleges
•	IITs
•	coaching institutes
•	professional companies

#### 18. Do I need admin permission to install VS Code?
Usually no, especially if you download the User Installer version.

#### 19. Why is VS Code not detecting my new Python installation?
Try these fixes:
✔ Restart VS Code
✔ Restart Windows
✔ Select interpreter manually
✔ Reinstall Python with PATH

#### 20. Does VS Code automatically update?
Yes — but updates are small and usually fast.



[Back to Table of Contents](#table-of-contents)

### 12. FAQ VS Code User Interface

[Back to Table of Contents](#table-of-contents)

Below are FAQs for each major panel, window, and section of the VS Code UI.

####  A. Activity Bar (Left-most slim column)

##### What is the Activity Bar?

It’s the thin vertical bar on the far left, showing icons like:  
📁 Explorer, 🔍 Search, 🔧 Run, 🧩 Extensions, etc.

##### What does it do?

It switches between different “views” inside VS Code.

##### Can I hide or show icons?

Yes → Right-click the Activity Bar → Show/Hide icons.

##### Can I move it to the bottom?

Yes → Settings → search “Activity Bar location” → Move.

#### B. Side Bar / Explorer Panel

##### What is the Explorer panel?

It shows all files and folders in your project.

##### My files are not appearing. Why?

You opened only a file, not the folder.  
Fix: File → Open Folder.

##### Folders look collapsed. How to expand?

Click the small ▸ arrow.

##### How to create a new file or folder?

Use the icons at the top:

*   📄 New File
*   📁 New Folder
*   🗑️ Delete

#### C. Editor Area (The main coding window)

##### What is the Editor Area?

The big central area where your code files open.

##### Can I open multiple files side by side?

Yes → Right-click a file tab → Split Right.

##### Why do I see two or three tabs of the same file?

You might have “Preview Mode” ON (italic filename).  
Double-click the file tab to keep it permanently open.

##### My text is too small/large.

Press Ctrl + + or Ctrl + -.

#### D. Tabs Bar (Top of the editor)

##### What are tabs?

Each open file has its own tab.

##### How to close many tabs quickly?

Right-click a tab → “Close All” or “Close Others”.

##### Can I reorder tabs?

Yes → drag them left/right.

#### E. Status Bar (Bottom bar)

##### What is the Status Bar?

The strip at the bottom showing useful info like:

*   Python version
*   Errors
*   Git branch
*   Encoding
*   Spaces/Tabs setting

##### Why is the bottom bar blue, purple, or red?

VS Code changes color depending on modes:

*   Blue → normal
*   Purple → debug mode
*   Red → admin mode

##### What does “Spaces: 4” or “Tabs: 4” mean?

It shows indentation settings.  
Click it to change indentation.

##### The Python interpreter on the left is wrong.

Click it → select the correct python.exe.

#### F. Panel (Bottom window for Terminal, Output, Problems)

##### What is the bottom “Panel”?

A multi-tab window containing:

*   Terminal
*   Problems
*   Output
*   Debug Console

##### My terminal disappeared!

Press Ctrl + \` (backtick) to toggle it.

##### Errors are shown under “Problems”. What should I do?

Click an error → VS Code jumps to that line.

##### “Output” tab shows nothing.

Some messages only appear when extensions use it.

#### G. Terminal Panel

##### Where is the terminal?

Bottom panel → select Terminal tab.

##### How to open a new terminal?

Click the ➕ icon.

##### Terminal shows wrong folder path.

You opened VS Code without the project folder.  
Fix: File → Open Folder.

##### How to change default terminal (PowerShell/CMD)?

Ctrl + Shift + P → Terminal: Select Default Profile

#### H. Problems Panel

##### What is this panel for?

It shows:

*   Errors
*   Warnings
*   Syntax issues

##### How do I fix the errors?

Click an error → It jumps to that line.

##### Why are there yellow warnings?

Warnings are suggestions, not errors.

#### I. Output Panel

##### What is the Output panel?

It shows logs from extensions (Python, Git, etc.)

##### Why can’t I see my program output here?

Your program’s output appears in Terminal, not Output.

#### J. Command Palette

##### What is the Command Palette?

A powerful search box opened by Ctrl + Shift + P.

##### What can it do?

Almost everything:

*   Change settings
*   Search commands
*   Install extensions
*   Format code
*   Switch themes

##### Why does everyone say “use the Command Palette”?

Because it’s the fastest way to do anything in VS Code.

#### K. Extensions View

##### Where do I find extensions?

Click the 🧩 Extensions icon in Activity Bar.

##### How do I install an extension?

Search → Click Install.

##### VS Code is slow after installing extensions.

Disable extra extensions → “Disable” button.

#### L. Settings

##### How do I open settings?

*   Press Ctrl + ,
*   OR use Command Palette: _Preferences: Open Settings_

##### What is the difference between User and Workspace settings?

*   User → affects all projects
*   Workspace → affects only current folder

##### Can I search for any setting?

Yes → type in the search bar.

#### M. Minimap (tiny map of code on right side)

##### What is that tiny vertical map?

It’s the minimap that shows a zoomed-out view of your code.

##### Can I turn it off?

Yes → Settings → “Minimap” → uncheck “Enabled”.

#### N. Breadcrumb Bar (top of editor)

##### What is Breadcrumbs?

Shows the file path and current function/class.

##### How to turn it on/off?

View → Toggle Breadcrumbs

#### O. Editor Layout Controls

##### How do I split the screen?

Right-click tab → Split Right OR  
Click the split icon (two rectangles).

##### Can I drag files between splits?

Yes, drag the tab.

#### P. Hover Tooltips / Auto Suggestions

##### Why do boxes pop up when I hover my mouse?

Those are tooltips explaining variables, functions, etc.

##### Can I disable them?

Settings → “Editor Hover” → Off.

#### Q. Welcome Page

##### How do I return to the Welcome screen?

Help → Welcome

##### How do I disable the welcome screen?

Uncheck “Show Welcome Page”.


#### Disclaimer

[Back to Table of Contents](#table-of-contents)











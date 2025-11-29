### Table of contents




### 1 Anaconda

#### 1.1 Introduction

##### 1.1.1  The Client–Server Model of Jupyter Notebook

Even though Anaconda and Jupyter Notebook run on your local computer, they still follow a client–server architecture internally.

That means:

•  Server = Python backend running on your computer

•  Client = Your web browser (Chrome/Edge/Firefox)

So you are still using your computer as:- Both the client AND the server

###### 1. Server: Jupyter Notebook Server

When you run:

jupyter notebook

or click “Launch” in Anaconda Navigator:

→ A small Python program called the Jupyter Notebook Server starts running in the background.

This server:

•  Runs on your machine

•  Manages files and notebooks

•  Executes Python code

•  Provides web pages for the interface

•  Communicates with the browser using WebSockets

The server usually runs at:

`http://localhost:8888`

localhost means:

Your own computer is acting as a server.

###### 2. Client: Your Web Browser

The Jupyter interface you see is just a website that your local server provides.

The browser:

•  Displays notebooks

•  Sends your code to the server

•  Receives output (text, images, errors)

•  Updates the notebook content

So the browser acts as a client UI.

1.1.2 Behind-the-Scenes: How Code Execution Works

•  Step-by-step internal process:

1.  You type Python code in a cell in your browser.

2.  Browser sends the cell code to the Jupyter server.

3.  The server sends the code to a kernel (usually IPython).

4.  The kernel executes the code.

5.  The result (text/plots/errors) is sent back to the server.

6.  The server sends the result to your browser.

7.  Browser displays the output in the notebook.

This process happens in milliseconds.

##### 1.1.3 What Is the Kernel (Internally)?

A kernel is a separate background process that executes code.

For Python notebooks, it is the IPython kernel:

•  Runs your Python code

•  Maintains variable state

•  Stores memory

•  Handles errors

•  Generates outputs

Even if the browser is closed, the kernel may keep running until stopped.

##### 1.1.4 Client–Server Role of Anaconda

Anaconda itself is not a client–server app, but:

It launches applications that use the model

It manages environments and packages that these apps need

•  Internally, Anaconda Navigator:

•  Runs as a local desktop GUI application

•  Acts as a launcher for tools

•  Starts Jupyter Notebook server when asked

•  Manages Python environments

Think of it like a control panel, not a server.

##### 1.1.5 How Everything Fits Together

•  ✔ When you start Jupyter from Anaconda:

1.  Anaconda starts the Jupyter Notebook Server

2.  The server listens on a port on your machine

Example: `localhost:8888`

3.  Your browser opens the interface

4.  The browser sends code → server → kernel

5.  Kernel executes code and returns results

6.  Browser displays the output

1.1.6 Why use a client–server model locally?

Even though everything is on your computer, this model gives benefits:

•  Benefit 1: Browser-based interface:- You don’t need a separate desktop app.

•  Benefit 2: Remote execution:- Same model works on remote servers (e.g., Google Colab, JupyterHub, cloud).

•  Benefit 3: Allows multiple clients:- Multiple browser tabs can talk to the same kernel.

•  Benefit 4: Language independence:- Kernel can be Python, R, Julia, etc., while browser stays the same.

#### 1.2 PART 1: Installing Anaconda (which includes Jupyter Notebook)

Anaconda is the easiest and recommended way for beginners to use Python and Jupyter Notebook.

##### 1.2.1 STEP 1 — Go to the Anaconda Website

###### 1.  Open your web browser (Chrome, Edge, Firefox).

###### 2.  Go to:

https://www.anaconda.com/download

##### 1.2.2 STEP 2 — Download the Windows Installer

###### 1.  Scroll to “Download Anaconda Distribution”.

###### 2.  Choose:

o  Operating System: Windows

o  Python Version: Choose `Python 3.x` (default is fine)

###### 3.  Click Download 64-bit Installer.

A file called something like:

`Anaconda3-2024.XX-Windows-x86_64.exe`

will start downloading.

##### 1.2.3 STEP 3 — Run the Installer

###### 1.  Locate the downloaded .exe file (usually in Downloads).

###### 2.  Double-click it to start the installation.

##### 1.2.4 STEP 4 — Initial Installer Screens

Click Next → Accept the license → Next.

##### 1.2.5 STEP 5 — Installation Type

Choose:

•  Just Me (recommended)

(Unless you know how admin installation works.)

Click Next.

1.2.6 STEP 6 — Choose Install Location

Leave it default:

`C:\Users\<yourname>\Anaconda3`

Click Next.

IMPORTANT STEP: PATH Checkbox

You will see two checkboxes:

✔ Add Anaconda to my PATH environment variable (NOT recommended—leave unchecked)

✔ Register Anaconda as my default Python → Check this one

Click Install.

##### 1.2.7 STEP 7 — Wait for Installation

This may take 5–10 minutes.

##### 1.2.8 STEP 8 — Finish

Click Next → Next → Finish.

You're done installing Anaconda!

#### 1.3 PART 2: Launching Jupyter Notebook (After Installation)

There are two easy methods.

##### 1.3.1 METHOD 1: Use Start Menu

1.  Press Start.

2.  Search Anaconda Navigator.

3.  Open it.

4.  On the home screen, click Launch under Jupyter Notebook.

✔ This opens Jupyter Notebook in your browser.

##### 1.3.2 METHOD 2: Use Anaconda Prompt

1.  Open Start → search Anaconda Prompt → open it.

2.  Type:

`jupyter notebook`

Press Enter.

✔ Jupyter Notebook will open in your browser.

1.3.3 You Now Have Jupyter Notebook Installed!

#### 1.4 PART 3: OPTIONAL — Installing Jupyter Notebook Without Anaconda

If you already have Python installed, you can install Jupyter with pip.

##### 1.4.1 STEP 1 — Check Python Installation

Open Command Prompt:

`python --version`

If Python is installed, continue.

1.4.2 STEP 2 — Install pip (if not already installed)

Usually pip comes with Python. Check:

`pip --version`

##### 1.4.3 STEP 3 — Install Jupyter Notebook

Run:

`pip install notebook`

##### 1.4.4 STEP 4 — Launch Notebook

jupyter notebook

#### 1.5 PART 4: Setting Up a Virtual Environment for Jupyter

(Optional but recommended)

##### 1.5.1 STEP 1 — Create Environment

`python -m venv myenv`

##### 1.5.2 STEP 2 — Activate Environment

Windows:

`myenv\Scripts\activate`

##### 1.5.3 STEP 3 — Install Jupyter Inside This Environment

`pip install notebook`

##### 1.5.4 STEP 4 — Launch Jupyter

`jupyter notebook`

#### 1.6 PART 5: Verifying Everything Works

In Jupyter:

1.  Click New → Python 3 (ipykernel).

2.  In the first cell, type:

`print("Hello Jupyter!")`

3.  Press Shift + Enter.

If it prints the message, your setup is perfect.

#### 1.7 Some more details of the local server when you launch Jupyter

When you start Jupyter Notebook, it automatically launches a local web server on your computer.

The link you see —

`http://localhost:8888/tree`

— is the address (URL) of that local server.

Here’s what each part means, in simple terms:

##### 1.7.1 `http://`

This means you are using the HTTP protocol, the same protocol used for regular websites.

##### 1.7.2 `localhost`

This means:

•  The server is running on your own computer, not on the internet.

•  `localhost` always refers to your own machine.

•  It is the hostname for IP address `127.0.0.1` (loopback address).

So opening localhost is like telling your browser:

"Connect to a server running on my own computer."

##### 1.7.3 `:8888 (Port Number)`

Computers can run many servers at the same time, each identified by a port.

Port `8888` means:

•  Jupyter Notebook server is listening for connections on port 8888.

•  If another service is already using 8888, Jupyter uses 8889, 8890, etc.

So:

`localhost:8888`

means:

“Connect to the server on my computer at port 8888.”

##### 1.7.4 `/tree`

This is the route or endpoint that displays the file browser view.

This view is called the Tree View because:

•  Your files are shown like a branching folder tree. The Jupyter interface you see (list of folders/files) is called the Tree View.

•  You can navigate up and down directories

•  You can open, delete, rename, or create new notebooks

So /tree loads:

The main home screen where you pick notebooks to open.

If you open a notebook, URL changes, for example:

•  `/notebooks/MyNotebook.ipynb`

•  `/edit/somefile.py`

•  `/terminals/1`

•  Tree = File Browser View

It refers to the directory tree — the list of folders and files on your computer, displayed in a hierarchical (tree-like) structure.

##### 1.7.5 Putting it all together

http://localhost:8888/tree means:

“Open the Jupyter Notebook server that is running on my own computer (localhost), using port 8888, and display the tree (file browser) interface.”

This is why everything runs locally — no internet needed.

##### 1.7.6 How the flow works

1.  You start Jupyter Notebook.

2.  It starts a Python-based server on your computer.

3.  That server listens on localhost:8888.

4.  Your browser opens the Jupyter UI at /tree.

5.  You interact with notebooks via your browser.

6.  The browser communicates with the Jupyter server.

7.  The server communicates with the Python kernel.

#### 1.8 You can think of Jupyter Notebook as having two main screens:

##### 1.8.1 Screen 1: The Tree View (Home Page)

URL: http://localhost:8888/tree

This is the first screen you see when Jupyter starts.

It functions like a file manager.

Here you can:

•  Browse your folders

•  See files and subfolders

•  Create new notebooks

•  Open existing notebooks

•  Upload files

•  Open terminals

It’s similar to a “home page” or “dashboard.”

##### 1.8.2 Screen 2: The Notebook Editor (When a notebook opens)

URL example:

http://localhost:8888/notebooks/myfile.ipynb

This is the actual interactive coding environment where you write Python code in cells.

In this screen, you get:

•  Menu bar

•  Code cells

•  Markdown cells

•  Output area

•  Kernel controls

This is where you run code.

##### 1.8.3 Relationship Between the Two Screens

•  The tree view is like a launcher.

•  The notebook editor is the actual work screen.

You always begin at Screen 1, unless you directly launch a notebook from the command line.

##### 1.8.4 Simplified Visual Explanation

```python
Start Jupyter

↓

Tree View (file browser)

↓ (open a file)

Notebook Editor (where you code)
```

#### 1.9 UI

1.9.1 Screen 1 — Tree View (the Jupyter home / file browser)

URL example: http://localhost:8888/tree

This is the first page Jupyter opens. It behaves like a simple file manager for the folder where you launched Jupyter.

Given below is the screen shot of Screen 1 with the “New” button clicked. It is from here that you select the various options to get the next screen. In most cases, you want to start a new Jupyter notebook, for which you may click the “Python 3 (ipykernel)”. But you may click other options as per your need.

##### 1.9.2 UI of screen 1

`.venv`

•  This is a virtual environment you created inside your project folder named .venv.

•  Jupyter detects it and shows it as a kernel.

•  If you select it, notebook cells will run using the Python interpreter inside .venv.

Useful when you want isolated packages for one project.

`Java`

•  This means you have a Java kernel installed (e.g., via IJava).

•  You can write and run Java code inside a notebook.

Example cell:
```java
System.out.println("Hello from Java!");
```
###### Python 3 (ipykernel)

•  This is the default Python kernel that comes bundled with Jupyter.

•  It uses your system-wide Python installation (not inside a venv).

•  This is the most common option for general use.

###### Text File

•  Creates a new blank .txt file.

•  Opens a simple text editor in the browser.

•  Useful for notes, config files, or documentation.

Folder

•  Creates a new folder in the current directory.

•  Helps you organize project files.

Terminal

•  Opens a Linux-like command-line terminal in your browser.

•  Lets you run:

o  pip install

o  git commands

o  virtual environment activation

o  python scripts

o  bash commands

This is very powerful and often used for managing environments.

1.9.3 XXX

###### 1 Header / Top Bar

•  Title — shows “Files” or the notebook server name.

•  Logo / Brand — small Jupyter logo and sometimes server info.

•  Useful for: Orienting you; no actions here typically.

###### 2 Toolbar (near top of page)

Common buttons you’ll see:

•  New → menu to create:

o  New Python 3 notebook (or other kernels)

o  New text file

o  New folder

o  New terminal (opens a shell tab)

•  Upload → upload files from your computer into the current folder

•  Refresh → re-scan the directory (useful when files were added externally)

•  Control / Shutdown (may appear in other views)

Tip: Use New → Notebook to quickly create a .ipynb ready to run.

###### 3 File / Folder list (the “tree”)

•  Shows all files and folders in the current directory.

•  Each row usually shows:

o  Filename (click to open)

o  Last modified time

o  File size (sometimes)

•  Right-click / three-dot menu on a file offers:

o  Open, Rename, Duplicate, Download, Delete, Move, Edit, View

o  For notebooks you may also see “Shutdown” (stops its kernel)

Tip: Clicking a folder enters it; clicking a notebook opens the editor (screen 2).

###### 4 Breadcrumb / Current path

•  Shows which folder you are viewing.

•  Click parents to go up one level.

###### 5 Running / Sessions (sometimes a tab or menu)

•  Running or Active sessions shows kernels/notebooks currently active.

•  From here you can shut down notebooks (stop their kernels) to free resources.

Why important: Closing a browser tab does not automatically stop the kernel — use this to shutdown.

###### 6 Search / Filter (if available)

•  Lets you find filenames in the current directory.

###### 7 Footer / Server info

•  May display the URL, token, or server messages.

•  Shows the directory that is being served (where files are stored).

##### 1.9.4 Screen 2 — Notebook Editor (the interactive coding screen)

URL example: http://localhost:8888/notebooks/myfile.ipynb

This is where you write and run code and see outputs.

###### 1 Browser URL & Notebook Name

•  The web page title usually contains the notebook name (myfile.ipynb).

•  Click the notebook name at top to rename it.

###### 2 Menu Bar (top row)

Typical menus:

•  `File` — New, Open, Make a copy, Rename, Save and Checkpoint, Download as (HTML, .py, .ipynb), Close and Halt

•  `Edit` — Cut/Copy/Paste cells, Find & Replace

•  `View` — Toggle toolbar/menu/line numbers

•  `Insert` — Insert cell above/below

•  `Cell` — Run Cells, Run All, Cell Type (Code / Markdown)

•  `Kernel` — Interrupt / Restart / Reconnect / Change kernel

•  `Help` — Keyboard shortcuts, docs, kernel info

Tip: File → Save and Checkpoint creates a backup checkpoint. Browser autosaves periodically.

###### 3 Notebook Toolbar (icons under menu)

Common buttons (left→right):

•  `Save` (floppy icon)

• ` Add cell, Cut/Copy/Paste cell, Move cell up/down`

•  `Run cell (▶) and Run all`

•  I`nterrupt kernel (stop), Restart kernel (⟳)`

###### 4 Kernel Status (top right)

•  Shows whether the kernel is Idle, Busy, or Disconnected.

•  Often a small circle: filled = busy, empty = idle.

•  Important actions:

o  Interrupt — stop a running cell (like Ctrl+C)

o  Restart — clear memory and restart Python kernel

Tip: If state is “Busy” and your code is stuck, click Interrupt or Restart.

###### 5 Cells — the basic building blocks

•  Two main cell types:

o  Code cells — contain executable Python code

o  Markdown cells — for formatted text, headings, lists, images

•  Each cell has its own run button (▶ on the left) and an execution number like In [1].

•  Outputs (below a code cell) show printed text, tables, plots, or errors.

•  Cell toolbar and actions:

•  Add new cell (above / below)

•  Change cell type (Code / Markdown)

•  Delete cell

•  Move cell up/down

6. Command Mode vs Edit Mode (keyboard behavior)

•  Edit mode (green border): typing inside a cell (press Enter to go into it).

•  Command mode (blue border): notebook-level commands (press Esc to enter).

•  Useful shortcuts:

o  Esc → Command mode

o  Enter → Edit mode

o  A (in Command) → Insert cell above

o  B (in Command) → Insert cell below

o  M → change to Markdown

o  Y → change to Code

o  D, D (press D twice) → delete cell

o  Shift+Enter → run cell and advance

o  Ctrl+Enter → run cell, do not advance

o  Alt+Enter → run cell and insert new cell below

o  H → show all keyboard shortcuts

###### 7 Output Area

•  Renders results: text prints, images/plots (matplotlib), HTML, DataFrames, etc.

•  Rich outputs are supported (interactive widgets, JavaScript).

Tip: If many outputs make notebook slow, Clear Output from Cell menu.

###### 8 Sidebar / Additional Panels (depends on interface)

•  File browser can reappear (JupyterLab has persistent sidebars; classic notebook may not).

•  Variable inspector / extensions may add panels (if installed).

###### 9 Status / Messages (bottom or header)

•  Kernel connection errors, long-running warnings, or autosave messages appear here.

###### 10 Checkpoints and Saving

•  Jupyter autosaves, but you can make a manual Checkpoint (File → Save and Checkpoint).

•  You can Download as .ipynb (or export to HTML/PDF).

#### 1.10 The New button in Jupyter’s Tree View.

#### 1.11 FAQ Frequently Asked Beginner Questions

##### 1.11.1 Do I need Anaconda to run Jupyter Notebook?

No, but it makes life easier.

##### 1.11.2 Will Jupyter run offline?

Yes.

##### 1.11.3 Is Anaconda free?

Yes, 100% free for personal and educational use.

##### 1.11.4 Does Jupyter Notebook save files?

Yes. Files are saved as .ipynb.

##### 1.11.5 Can I uninstall Anaconda and keep Python?

Yes — both are separate.

#### 1.12 VVV

#### 1.13 VVV

### 2 Some additional information

#### 2.1 Magic commands

Magic commands in Jupyter Notebook are special commands that start with % or %% and are not part of standard Python, but are added by IPython to make your workflow easier.

They help you manage the notebook, run system commands, measure performance, load files, debug, profile code, and more — all without leaving Jupyter.

Magic commands are like shortcuts or superpowers inside Jupyter.

They help you perform tasks such as:

✔ Checking your directory

✔ Timing your code

✔ Loading external scripts

✔ Running OS commands

✔ Controlling the Jupyter environment

✔ Displaying plots

✔ Debugging

✔ Saving variables across notebooks

They come in two types.

##### 2.1.1 Line Magics (start with %)

These run on a single line.

Example:-

`%pwd  # print working directory`

`%ls  # list files`

##### 2.1.2 Common Line magic commands in tabular form

  
  

  

| Name | Format | What It Does | Simple Example |
| --- | --- | --- | --- |
| %pwd | %pwd | Shows current working directory | %pwd |
| %ls | %ls | Lists files in the current directory | %ls |
| %cd | %cd foldername | Changes directory | %cd data |
| %who | %who | Lists defined variables in workspace | %who |
| %whos | %whos | Shows variables with details (type, size, etc.) | %whos |
| %reset | %reset | Clears all variables from workspace | %reset -f |
| %run | %run script.py | Runs a Python script inside the notebook | %run myfile.py |
| %time | %time statement | Measures execution time of a single statement | %time x = sum(range(100000)) |
| %timeit | %timeit statement | Runs the statement multiple times to give accurate timing | %timeit x = sum(range(100000)) |
| %matplotlib inline | %matplotlib inline | Displays plots inside notebook | %matplotlib inline |
| %store | %store varname | Saves a variable for use in another notebook/session | %store x |
| %history | %history | Shows command history | %history |
| %pip | %pip install package | Installs Python packages directly from notebook | %pip install numpy |
| %conda | %conda install package | Installs packages using conda from notebook | %conda install pandas |

##### 2.1.3 Cell Magics (start with %%)

These apply to the whole cell.

Example:

`%%time`

 entire cell is timed

```python
x = 0

for i in range(1000000):

x += i
```

##### 2.1.4 Common Cell magic commands in tabular form

  

| Name | Format | What It Does | Simple Example |
| --- | --- | --- | --- |
| %%time | %%time | Measures execution time of the entire cell | %%timex = [i*i for i in range(100000)] |
| %%timeit | %%timeit | Runs full cell many times & averages the timing | %%timeitx = [i*i for i in range(100000)] |
| %%bash | %%bash | Runs the entire cell as Bash shell commands | %%bashecho "Hello"\nls |
| %%python | %%python | Forces execution using Python interpreter (useful in multi-kernel setups) | %%pythonprint("Hello") |
| %%html | %%html | Renders HTML content in output | %%html<h1>Hello</h1> |
| %%markdown | %%markdown | Renders Markdown as formatted output | %%markdown\n# Title |
| %%writefile | %%writefile filename.py | Writes the content of the cell to a file | %%writefile test.py\nprint("Hello") |
| %%capture | %%capture varname | Captures output (stdout, stderr) into a variable | %%capture outprint("Hidden") |
| %%latex | %%latex | Renders LaTeX math | %%latexE=mc^2 |
| %%javascript | %%javascript | Runs JavaScript inside notebook | %%javascriptalert("Hi!") |

### 3 Advanced concepts

#### 3.1 Flowchart

##### 3.1.1 Explanation

###### A — Anaconda Navigator

Block: A[Anaconda Navigator]

This is the graphical launcher that comes with Anaconda.

You click an icon → Navigator opens → you see apps like Jupyter Notebook, Spyder, VS Code, etc.

Meaning:- The entire workflow starts when you launch Jupyter Notebook from Anaconda Navigator.

###### A → B — Starting the Notebook Server

Block: B[Starts Jupyter Notebook Server]

When you click “Launch” → Navigator runs the command:

jupyter-notebook

This starts something called the Jupyter Notebook Server.

The server is a Python program running locally on your computer.

###### B → C — Jupyter Server Running on Localhost

Block: C[Jupyter Server Running on Localhost]

The Jupyter server starts on something like:

http://localhost:8888

“localhost” means your own computer.

This server manages:

•  Notebook files

•  Saving

•  Communication with kernels

•  Security tokens

•  Sessions

###### C → D — Browser Opens Notebook Interface

Block: D[Browser Opens Notebook Interface]

After the server starts, your web browser opens automatically.

This web page is the Jupyter Dashboard (list of notebooks) and later the Notebook Editor.

Even though it looks like a website, the entire thing runs on your computer, not on the internet.

###### D → E — User Writes Code

Block: E[User Writes Code in Cell]

Inside the browser, you type:
```python
a = 10

a + 20
```

This is just text until you run the cell.

###### E → F — Browser Sends Code to Server

Block:

F[Browser Sends Code to Server]

When you press Shift+Enter, the browser sends your code to the Jupyter server using HTTP/WebSocket.

The server receives something like:

"Run cell with code: a + 20"

###### F → G — Server Sends Code to Kernel

Block:

G[Server Sends Code to Kernel]

The Jupyter server forwards the code to a kernel.

The kernel is a Python process running separately:

python.exe -m ipykernel

This is what actually executes your code.

###### G → H — Kernel Executes the Code

Block: H[Kernel Executes Python Code]

The kernel:

•  parses your Python

•  executes it

•  maintains variable states

•  stores your session memory

###### H → I — Python Produces Output

Block:

I[Python Produces Output]

This is simply the result of your code:

30

or a graph, or a printed message.

10. I → J — Kernel Sends Output to Server

Block:

J[Kernel Sends Output to Server]

After executing the code, the kernel returns:

•  the output

•  any errors

•  stdout (print)

•  rich outputs (plots, HTML, images)

It sends this back in a structured JSON message.

###### J → K — Server Sends Output to Browser

Block:

K[Server Sends Output to Browser]

The Jupyter server receives the kernel's JSON output and forwards it to your browser.

###### K → L — Browser Displays Output

Block:

L[Browser Displays Output in Notebook]

The browser renders the output below your code cell.

This completes the cycle:

1.  You write code

2.  It travels through server → kernel

3.  Kernel executes

4.  Result travels back

5.  Browser displays it

#### 3.2 Where does Jupyter Stores Kernels

Common paths:

•  Linux / Mac:

`~/.local/share/jupyter/kernels/`

•  Windows:

`C:\Users\<username>\AppData\Roaming\jupyter\kernels\`

Each kernel has a folder with:

•  kernel.json

•  an icon

•  the executable path

3.3 SSS

3.4 CCC

3.5 qqq

4 XXX






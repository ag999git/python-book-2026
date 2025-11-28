

## VS Code
### 1.1 VS Code basics
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


### 2.1 First-time Setup for Beginners
When VS Code launches:
    
#### 2.1.1 You may see:
    
*   “Do you trust this author?” → Click **Yes**
*   “Would you like to install recommended extensions?” → Optional
  VS Code opens with a **welcome page** that includes:
    *   A "Get Started" guide
    *   Themes (light/dark)
    *   Buttons to create/open files
    
### 3 Understanding the VS Code Interface (Beginner-Friendly)

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






### TEST

















# Gemini AI Debugger

## Overview
Gemini AI Debugger is an advanced debugging assistant designed to analyze, debug, and improve Python scripts. It integrates with **Google's Gemini AI** to identify errors, suggest modifications, and optimize code while maintaining execution integrity. Additionally, it offers **GitHub integration** for seamless file management and version control.

## Features
- **AI-Powered Debugging**: Detects syntax and logical errors in Python code.
- **Automated Fixes**: Suggests and applies fixes while preserving core functionality.
- **Code Optimization**: Enhances readability, efficiency, and maintainability.
- **GitHub Integration**: Supports repository selection, file uploads, and commits.
- **User-Friendly UI**: Provides an interactive interface using **Tkinter**.
- **Versioning Support**: Creates a `_v2` version of the file for modifications.
- **Changes Log**: Maintains a log of all modifications for transparency.

#Create a `.env` file with your API keys:
   ```
   API_KEY=your_gemini_api_key
   Github_user=your_github_username
   Github_accessToken=your_github_access_token
   ```

## Usage
1. Run the script:
   ```sh
   python script.py
   ```
2. Select a Python file to debug.
3. Enter debugging queries such as:
   - "Find all bugs in this script."
   - "Optimize this function for efficiency."
   - "Modify this script to handle exceptions."
4. The AI will analyze the script and provide debugging reports and fixes.
5. Apply fixes and merge them into the original file if desired.
6. Optionally, commit the changes to GitHub.
7. Type `exit` to close the program and optionally delete the modified file.

## Sample Use Case
### **User Input:**
```sh
Enter a prompt: Find all bugs in my script.
```

### **AI-Generated Output:**
```python
Errors Found:
- Logical Errors: 2
- Syntax Errors: 1
- Suggestions: 3

Error Details:
- Line 10: SyntaxError - Missing colon after function definition.
  Solution: Add a colon at the end of the line.

- Line 25: LogicalError - Infinite loop condition detected.
  Solution: Introduce a termination condition.

Code Fix:
```python
# Corrected Code
...
```

Changes logged in `script_changes.txt`.
```

## GitHub Integration
- **List Repositories**: View available GitHub repositories.
- **Create Repository**: Create a new repository from the UI.
- **Upload File**: Commit the modified script to the selected repository.

## Notes
- The script limits conversation history to the last 5 exchanges for context management.
- Ensure valid API credentials are set in the `.env` file.



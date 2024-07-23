# Dev_Setup
Setup Development Environment

#Assignment: Setting Up Your Developer Environment

#Objective:
This assignment aims to familiarize you with the tools and configurations necessary to set up an efficient developer environment for software engineering projects. Completing this assignment will give you the skills required to set up a robust and productive workspace conducive to coding, debugging, version control, and collaboration.

#Tasks:

1. Select Your Operating System (OS):
   Choose an operating system that best suits your preferences and project requirements. Download and Install Windows 11. https://www.microsoft.com/software-download/windows11

2. Install a Text Editor or Integrated Development Environment (IDE):
   Select and install a text editor or IDE suitable for your programming languages and workflow. Download and Install Visual Studio Code. https://code.visualstudio.com/Download
3. Set Up Version Control System:
   Install Git and configure it on your local machine. Create a GitHub account for hosting your repositories. Initialize a Git repository for your project and make your first commit. https://github.com

4. Install Necessary Programming Languages and Runtimes:
  Instal Python from http://wwww.python.org programming language required for your project and install their respective compilers, interpreters, or runtimes. Ensure you have the necessary tools to build and execute your code.

5. Install Package Managers:
   If applicable, install package managers like pip (Python).

6. Configure a Database (MySQL):
   Download and install MySQL database. https://dev.mysql.com/downloads/windows/installer/5.7.html

7. Set Up Development Environments and Virtualization (Optional):
   Consider using virtualization tools like Docker or virtual machines to isolate project dependencies and ensure consistent environments across different machines.

8. Explore Extensions and Plugins:
   Explore available extensions, plugins, and add-ons for your chosen text editor or IDE to enhance functionality, such as syntax highlighting, linting, code formatting, and version control integration.

9. Document Your Setup:
    Create a comprehensive document outlining the steps you've taken to set up your developer environment. Include any configurations, customizations, or troubleshooting steps encountered during the process.
    ## Setting Up a Developer Environment

 1. **Choosing the Development Environment**
   - **Operating System**: Ubuntu 22.04 LTS
   - Integrated Development Environment (IDE)**: Visual Studio Code (VSCode)

 2.  Installing the Operating System**
   - Ubuntu 22.04 LTS**:
     - Download the ISO file from the [official Ubuntu website](https://ubuntu.com/download/desktop).
     - Create a bootable USB drive using tools like Rufus or Etcher.
     - Boot from the USB drive and follow the installation instructions.

 3. Initial System Setup
   - Update and Upgrade System Packages
     ```bash
     sudo apt update
     sudo apt upgrade
     ```
   - Installing Common Utilities
     ```bash
     sudo apt install -y curl wget git build-essential
     ```

 4. Installing Development Tools
   -Visual Studio Code
     - Download the .deb package from the [official VSCode website](https://code.visualstudio.com/Download).
     - Install VSCode:
       ```bash
       sudo dpkg -i code*.deb
       sudo apt install -f  
       ```
   - Git
     ```bash
     sudo apt install git
     ```
     - Configure Git:
       ```bash
       git config --global user.name "Your Name"
       git config --global user.email "your.email@example.com"
       ```

 5. Setting Up Version Control
- GitHub
     - Create a GitHub account if you don’t have one.
     - Generate SSH keys:
       ```bash
       ```
       - Add the SSH key to the ssh-agent:
         ```bash
         eval "$(ssh-agent -s)"
         ssh-add ~/.ssh/id_ed25519
         ```
       - Add the SSH key to your GitHub account by copying the key and pasting it into your GitHub SSH settings:
         ```bash
         cat ~/.ssh/id_ed25519.pub
         ```

 6. Programming Languages and Frameworks
   - Python
     ```bash
     sudo apt install python3 python3-pip
     ```
     - Create a virtual environment:
       ```bash
       python3 -m venv myenv
       source myenv/bin/activate
       ```
     - Install necessary packages:
       ```bash
       pip install numpy pandas flask django
       ```
   - Node.js and np
     ```bash
     curl -sL https://deb.nodesource.com/setup_16.x | sudo -E bash -
     sudo apt install -y nodejs
     ```
   - Java:
     ```bash
     sudo apt install openjdk-11-jdk
     ```

 7. Database Setup

     ```bash
     sudo apt install postgresql postgresql-contrib
     sudo -i -u postgres
     createuser --interactive
     createdb mydatabase
     ```

 8. Configuring IDE Extensions
   - VSCode Extensions
     - Python
     - Prettier - Code formatter
     - ESLint
     - GitLens
     - Docker
     - Live Server
   - Settings
     - Configure settings in `settings.json`:
       ```json
       {
         "editor.tabSize": 4,
         "editor.formatOnSave": true,
         "files.autoSave": "afterDelay",
         "python.pythonPath": "myenv/bin/python"
       }
       ```

 9. Containerization
   - Docker
     ```bash
     sudo apt install docker.io
     sudo systemctl start docker
     sudo systemctl enable docker
     sudo usermod -aG docker ${USER}
     ```
     - Verify Docker installation:
       ```bash
       docker --version
       ```
   - Docker Compose
     ```bash
     sudo curl -L "https://github.com/docker/compose/releases/download/1.29.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
     sudo chmod +x /usr/local/bin/docker-compose
     ```

 10. Troubleshooting Steps
   - Fixing Dependency Issues
     - If you encounter dependency issues, use:
       ```bash
       sudo apt --fix-broken install
       ```
   - Resolving Permission Issues
     - If you face permission issues with Docker, ensure the user is added to the Docker group:
       ```bash
       sudo usermod -aG docker ${USER}
       ```
   - Common Python Errors
     - If there are issues with pip packages, ensure `pip` is updated:
       ```bash
       pip install --upgrade pip
       ```

 11. Customizations
   - Bash Aliases
     - Add useful aliases to `.bashrc` or `.zshrc`:
       ```bash
       alias ll='ls -alF'
       alias la='ls -A'
       alias l='ls -CF'
       alias gs='git status'
       alias gd='git diff'
       ```
     - Apply changes:
       ```bash
       source ~/.bashrc  # or ~/.zshrc
       ```
   - Prompt Customization
     - Customize the command prompt by adding the following to `.bashrc`:
       ```bash

#Deliverables:
- Document detailing the setup process with step-by-step instructions and screenshots where necessary.
- A GitHub repository containing a sample project initialized with Git and any necessary configuration files (e.g., .gitignore).
- A reflection on the challenges faced during setup and strategies employed to overcome them.

#Submission:
Submit your document and GitHub repository link through the designated platform or email to the instructor by the specified deadline.

#Evaluation Criteria:**
- Completeness and accuracy of setup documentation.
- Effectiveness of version control implementation.
- Appropriateness of tools selected for the project requirements.
- Clarity of reflection on challenges and solutions encountered.
- Adherence to submission guidelines and deadlines.

Note: Feel free to reach out for clarification or assistance with any aspect of the assignment.

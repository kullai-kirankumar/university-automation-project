# university-automation-project
This repository contains example code for the Behavior-Driven Python with pytest-bdd course from Test Automation University. There is a branch for each chapter of the course showing the state of the code at the completion of the chapter.

#Repository Purpose
The best way to learn pytest is through hands-on coding. In the first lesson of the course, you will create a new Python project for test cases. (That project will not be the same as this repository.) Each chapter then introduces new concepts and provides coding instructions for your project. If you code along with each chapter, then you will have a complete, functioning test automation project by the end of the course.

This repository provides all example code for the project. If you get stuck while building your own project, compare your code to the example code in this repository. However, try to avoid blindly copying code from the repository into your project. Take the time to learn the concepts and code presented in each chapter.

#Repository Branches
Each chapter/* branch contains the state of the code for each chapter
The main branch contains the final state of the code at the end of the course
Python Setup
Python setup can be complicated. This section documents how to set up your machine for Python test automation development.

Python Installation and Tools
You can complete this course using any OS: Windows, macOS, Linux, etc.

This course requires Python 3. You can download the latest Python version from Python.org. Follow the appropriate installation instructions for your operating system.

You should have basic Python programming skills before attempting this course. Learning the language is always a prerequisite for learning automation. If you need help learning Python, check out this article: How Do I Start Learning Python?

You should also have a good Python editor/IDE. Good choices include PyCharm and Visual Studio Code.

You will also need Git if you want to clone this repository locally. If you are new to Git, try learning the basics.

For Web UI tests, install the appropriate browser and WebDriver executable. These tests use Firefox and geckodriver.

Python Installation Troubleshooting
Unfortunately, installing Python properly can be complicated, especially if Python was previously installed on your machine. To verify your Python installation, enter python --version at the command line. You should see the proper version printed.

If the python command doesn't work or doesn’t print the expected version number, then try using the python3 command instead. If that still doesn't work, then the correct Python installation might not be included in your system path. Find the directory into which Python was installed, manually add it to the system path, relaunch the command line, and try running Python again.

System Path Instructions for Windows
System Path Instructions for macOS
System Path Instructions for Linux
Python Packages
This course will use a handful of third-party packages that are not part of the Python Standard Library. They must be installed separately using pip, the standard Python package installer. You can install them all before you create your test project, or you can install them as you complete each chapter in the course.

To install each package, enter pip install <package-name> at the command line. For example: pip install pytest. If you already have a package installed but need to upgrade its version, run pip install --upgrade <package-name>.

Please note that if you need to use the python3 command to run Python, then you might also need to use the pip3 command in lieu of pip.

Virtual Environments
Running pip install will install the pytest package globally for the whole system. Installing Python packages globally is okay for this course, but it typically isn't a best practice in the "read world." Instead, each project should manage its own dependencies locally using a virtual environment. Virtual environments let projects avoid unnecessary dependencies and version mismatches.

For simplicity, this course will not use or teach virtual environments. If you would like to learn virtual environments on your own, then RealPython's article Python Virtual Environments: A Primer is an excellent place to start.

Package Versions
The requirements.txt file contains the versions for each package used in this course.

Running Tests
To run the example tests from the command line, run python -m pytest from the project root directory. This command will discover and run all tests in the project.

You can also run tests using the shorter pytest command. However, I recommend always using the lengthier python -m pytest command. The lengthier command automatically adds the current directory to sys.path so that all modules in the project can be discovered.

The pytest command has several command line options. Course material will cover many of them. Check out the Usage and Invocations page for complete documentation.

Warning: If you attempt to run tests from this example project, make sure to checkout the correct branch first!

Table of Contents
Overview

Features
Technologies Used
Setup and Installation
Running the Project
CI/CD Pipeline
Deployment
Environment Variables
Docker Setup
Contributing
License

Overview
This project is a personal portfolio built with React.js, showcasing my skills, projects, and experience. The portfolio features a CI/CD pipeline for seamless deployment and updates.

Features
Responsive Design: Adapts to different screen sizes for an optimal viewing experience on any device.
Interactive Project Showcases: Highlight projects with detailed descriptions and visual elements.
Contact Form Integration: Enables visitors to get in touch easily.
Smooth Navigation and Transitions: Provides a seamless user experience.
Automated CI/CD Pipeline: Ensures continuous integration and deployment of updates.

Technologies Used
Frontend: React.js, HTML, CSS, JavaScript
CI/CD: GitHub Actions
Deployment: Netlify
Setup and Installation
Prerequisites
Node.js and npm installed
Git installed
Installation Steps
Clone the repository:

git clone https://github.com/Alemu2502/reactjs-portfolio.git
cd reactjs-portfolio
Install dependencies:

npm install
Running the Project
Development Mode
To run the project in development mode:

npm start
Production Build
To create a production build:

npm run build
CI/CD Pipeline
This project uses GitHub Actions for continuous integration and deployment. The CI/CD pipeline includes steps for:

Checking out the code
Caching Node modules
Setting up Node.js
Installing dependencies
Running tests (commented out for now)
Building the project
Deploying to Netlify

Deployment
The frontend is deployed using Netlify. The deployment configuration is handled in the GitHub Actions workflow.

Environment Variables
Make sure to set the following environment variables for proper configuration:

Frontend (set in Netlify):

VITE_SERVICE_ID
VITE_TEMPLATE_ID
VITE_USER_ID
VITE_GITHUB
VITE_FACEBOOK
VITE_LINKEDIN
VITE_TWITTER

Docker Setup
Prerequisites
To use Docker, ensure you meet the following prerequisites:

WSL version: WSL 1.1.3.0 or later

Operating System:

Windows 11 64-bit: Home or Pro version 22H2 or higher, or Enterprise or Education version 22H2 or higher.
Windows 10 64-bit: Minimum required is Home or Pro 22H2 (build 19045) or higher, or Enterprise or Education 22H2 (build 19045) or higher.

Hardware:

64-bit processor with Second Level Address Translation (SLAT)
4GB system RAM
Enable hardware virtualization in BIOS. For more information, see Virtualization.

Installing Docker Desktop
Download Docker Desktop:

Docker Desktop for Windows: https://desktop.docker.com/win/stable/Docker%20Desktop%20Installer.exe

Docker Desktop for Mac: https://desktop.docker.com/mac/stable/Docker.dmg

Install Docker Desktop: Follow the installation instructions for your operating system.

Check Docker Version: Open your Command Prompt or PowerShell and run:

docker --version
Enabling WSL 2 (Windows Users)
Enable Windows Subsystem for Linux: Open PowerShell as Administrator and run:

wsl --install
sudo apt-get update
sudo apt-get upgrade
Enable Virtual Machine Platform: Still in PowerShell, run:

dism.exe /online /enable-feature /featurename:VirtualMachinePlatform /all /norestart
Install Docker in WSL: After setting up WSL, install Docker:

sudo apt-get install docker.io
Add User to Docker Group (optional): If you want to run Docker commands without sudo, add your user to the Docker group:

sudo usermod -aG docker $USER
For more information on setting up WSL 2 with Docker Desktop, see WSL Documentation: https://docs.microsoft.com/en-us/windows/wsl/

> Note: Docker only supports Docker Desktop on Windows for those versions of Windows that are still within Microsoft’s servicing timeline. Docker Desktop is not supported on server versions of Windows, such as Windows Server 2019 or Windows Server 2022. For more information on how to run containers on Windows Server, see Microsoft's official documentation.

> Important: To run Windows containers, you need Windows 10 or Windows 11 Professional or Enterprise edition. Windows Home or Education editions only allow you to run Linux containers.

Contributing
Feel free to contribute to this project by creating a pull request or opening an issue.

License
This project is licensed under the MIT License.

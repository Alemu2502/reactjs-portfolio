
Overview
This project is a personal portfolio built with React.js, showcasing my skills, projects, and experience. The portfolio features a CI/CD pipeline for seamless deployment and updates.

Table of Contents
1. [Overview](#overview) 
2. [Features](#features) 
3. [Technologies Used](#technologies-used) 
4. [Setup and Installation](#setup-and-installation)
5. [Running the Project](#running-the-project) 
6. [CI/CD Pipeline](#cicd-pipeline) 
7. [Deployment](#deployment) 
8. [Environment Variables](#environment-variables)
9. [Docker Setup](#docker-setup) 
10. [Contributing](#contributing)
11. [License](#license)

Features:
Responsive design
Interactive project showcases
Contact form integration
Smooth navigation and transitions
Automated CI/CD pipeline for deployment

Technologies Used:
Frontend: React.js, HTML, CSS, JavaScript
CI/CD: GitHub Actions
Deployment: Netlify

Setup and Installation:
Prerequisites
Node.js and npm installed
Git installed

Installation Steps
Clone the repository:
bash
git clone https://github.com/Alemu2502/reactjs-portfolio.git
cd reactjs-portfolio
Install dependencies:

bash
npm install
Running the Project
Development Mode
To run the project in development mode:
bash
npm start
Production Build
To create a production build:

bash
npm run build

CI/CD Pipeline:
This project uses GitHub Actions for continuous integration and deployment. The CI/CD pipeline includes steps for:

Checking out the code
Caching Node modules
Setting up Node.js
Installing dependencies
Running tests (commented out for now)
Building the project
Deploying to Netlify

Deployment:
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

Download Docker Desktop:

Docker Desktop for Windows: https://desktop.docker.com/win/stable/Docker%20Desktop%20Installer.exe(use in this way for all other links )

Docker Desktop for Mac: https://desktop.docker.com/mac/stable/Docker.dmg
 check docker version
 open your cmd or power shell 
 docker --version

 Installing Docker Desktop
Follow the installation instructions for your operating system.

check Virtualization is Enabled in your bios settings
Enabling WSL 2 (Windows Users)
Enable Windows Subsystem for Linux:

Open PowerShell as Administrator and run:
wsl --install 
Run wsl -l -v in PowerShell to see the installed distributions and versions.
sudo apt-get update
sudo apt-get upgrade
then now we can install docker in ubuntu or wsl 
sudo apt-get install docker.io

and we should your user to the docker group  to run docker comands without sudo if you want else skip this



For more information on setting up WSL 2 with Docker Desktop, see WSL Documentation: https://docs.microsoft.com/en-us/windows/wsl/

> Note: > Docker only supports Docker Desktop on Windows for those versions of Windows that are still within Microsoft’s servicing timeline. Docker Desktop is not supported on server versions of Windows, such as Windows Server 2019 or Windows Server 2022. For more information on how to run containers on Windows Server, see Microsoft's official documentation.

> Important: > To run Windows containers, you need Windows 10 or Windows 11 Professional or Enterprise edition. Windows Home or Education editions only allow you to run Linux containers.

Contributing
Feel free to contribute to this project by creating a pull request or opening an issue.

License
This project is licensed under the MIT License.




CI/CD Pipeline
This project uses GitHub Actions for Continuous Integration and Continuous Deployment (CI/CD). The workflow automates the process of building, testing, and deploying the application to Netlify.

Workflow Overview
Trigger: The workflow triggers on every push or pull request to the main branch.

Steps:

Checkout the code.

Cache dependencies.

Set up the Node.jsenvironment.

Install project dependencies using npm ci.

Run tests to ensure code quality.

Build the project.

Deploy the project to Netlify.

Benefits
Efficiency: The workflow completes in around 25 seconds, ensuring fast and reliable deployments.

Quality Assurance: Tests run before deployment to catch any issues early.

Best Practices: Implements industry best practices such as dependency caching and environment setup.
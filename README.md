Table of Contents
1. [Overview](#overview) 
2. [Features](#features) 
3. [Technologies Used](#technologies-used) 
4. [Setup and Installation](#setup-and-installation)
5. [Running the Project](#running-the-project) 
6. [CI/CD Pipeline](#cicd-pipeline) 
7. [Deployment](#deployment) 
8. [Environment Variables](#environment-variables)
9. [Emailjs Integration](#emailjs-integration) 
10. [Clean-Up Old Workflows](#clean-up-old-workflows)
11. [Contributing](#contributing)
12. [Contact](#contact)
13. [License](#license)
14. [Conclusion](#conclusion)

### Overview

This project is a personal portfolio built with React.js, showcasing my skills, projects, and experience. The portfolio features a CI/CD pipeline for seamless deployment and updates.

### Features

1. Responsive Design: Adapts to different screen sizes for an optimal viewing experience on any device.
2. Interactive Project Showcases: Highlight projects with detailed descriptions and visual elements.
3. Contact Form Integration: Enables visitors to get in touch easily.
4. Smooth Navigation and Transitions: Provides a seamless user experience.
5. Automated CI/CD Pipeline: Ensures continuous integration and deployment of updates.

### Technologies Used

1. Frontend: React.js, HTML, CSS, JavaScript
2. CI/CD: GitHub Actions
3. Deployment: Netlify(The frontend of this project is deployed using Netlify. If you haven't created a Netlify account yet, you can sign up for free [here](https://app.netlify.com/signup))

### Setup and Installation

Prerequisites
1. Node.js and npm installed
2. Git installed
3. Installation Steps

Clone the repository:

git clone https://github.com/Alemu2502/reactjs-portfolio.git

   cd reactjs-portfolio

Install dependencies:

   npm install

### Running the Project

Development Mode
  To run the project in development mode:

  npm start

  Production Build
  To create a production build: 

   npm run build

### CI/CD Pipeline

This project uses GitHub Actions for continuous integration and deployment.

 # The CI/CD pipeline includes steps for:

1. Checking out the code
2. Caching Node modules
3. Setting up Node.js
4. Installing dependencies
5. Running tests (commented out for now)
6. Building the project
7. Deploying to Netlify

### Deployment

The frontend is deployed using Netlify. The deployment configuration is handled in the GitHub Actions workflow.

### Environment Variables

Frontend (set in Netlify): In this project, i utilize several environment variables to 
maintain consistency and manage configurations. These variables include both essential 
service identifiers and social media links. While the social media links are stored in 
the environment file for consistency, they are intended to be publicly accessible. 
If you prefer, you can use them as public values.

Here are the environment variables used:

 1. VITE_SERVICE_ID
 2. VITE_TEMPLATE_ID
 3. VITE_USER_ID
 4. VITE_GITHUB
 5. VITE_FACEBOOK
 6. VITE_LINKEDIN
 7. VITE_TWITTER

To set these variables in Netlify, you can navigate to the site's settings and add them under the "Build & Deploy" section.

### Emailjs Integration

EmailJS Integration

Overview

This project utilizes EmailJS to handle the contact form submissions. EmailJS allows you to send emails directly from your JavaScript code without needing a server.

Why EmailJS?

No Server Required: 
EmailJS provides a serverless solution to send emails from your client-side application.

Easy Setup:
 With minimal configuration, you can integrate EmailJS and start sending emails.

Secure: 
EmailJS handles the email sending process securely, so you don't need to expose your SMTP credentials.

Setup and Integration
Follow these steps to integrate EmailJS with your contact form:

Create an Account: If you don't have an EmailJS account, sign up [here](https://dashboard.emailjs.com/sign-up)

Create a New Email Service:

After logging in, go to the Email Services section and create a new email service.

Add your email provider (e.g., Gmail, Outlook) and connect it.

Create an Email Template:

Navigate to the Email Templates section and create a new template.

Define the template parameters and structure (e.g., subject, body).

Get Your User ID(public key), Service ID, and Template ID:

Go to the Integration section and copy your User ID.

Note down your Service ID and Template ID from the Email Services and Templates sections, respectively.

so after that Add these Environment Variables to github secrets.

Testing

Local Testing: 
Run your project locally and test the contact form to ensure it sends emails correctly.

Deployed Testing: 

After deploying your project (e.g., on Netlify), test the contact form again to ensure it works in the live environment.

## Clean-Up Old Workflows 

To maintain a clean and manageable CI/CD history, i implement a periodic clean-up process. This process involves: 
1. Scheduled Clean-Up:
 Every moth, old workflows that have been resolved and documented are deleted. This helps keep the workflow history clean and efficient. 
 2. Automated Clean-Up: 
 I use a GitHub Actions workflow to automate the clean-up process. The workflow runs every moth and deletes old workflows. The clean-up workflow found [here](.github/workflows/cleanup.yml). 
 3. Archiving: 
 Significant issues and their resolutions are documented and archived before deletion. By following these best practices, we ensure that our CI/CD pipeline remains efficient and clutter-free. If you have any suggestions or improvements, feel free to open a pull request or contact me. 

but fisrt you should Checking and Updating GitHub Token Permissions
To ensure your GitHub Actions workflow can run correctly, follow these steps to check and update the GITHUB_TOKEN permissions:

Steps to Check and Update GITHUB_TOKEN Permissions:

Navigate to Your Repository Settings:

1. Go to your GitHub repository.
2. Click on the "Settings" tab.
3. Access Actions Settings:

In the left sidebar, scroll down to find and click on "Actions".

1. General Settings:
2. Under the "Actions" section, click on "General".

Update Workflow Permissions:

Look for the "Workflow permissions" section.

Ensure that the "Read and write permissions" option is selected. This setting allows the GITHUB_TOKEN to perform read and write operations, such as deleting workflow runs.

### Contributing

Feel free to contribute to this project by creating a pull request or opening an issue.

### Contact
For any questions, suggestions, or collaboration opportunities, feel free to connect with me through the following channels:

Email: alemu4617@gmail.com

Portfolio: https://my-react-app-o8w4.onrender.com/  - Explore my projects and learn more about my work.

Docker Hub: https://hub.docker.com/repository/docker/alemu2502/my-react-docker-app - Access the Docker images for this project.

LinkedIn:   https://www.linkedin.com/in/Alemu2502 - Connect with me professionally.

Facebook: https://www.facebook.com/alemu.molla.1806 

Twitter: https://twitter.com/ALEXSEPPRO
  - Follow me for updates and insights.

### License

 MIT License

Copyright (c) 2024 Alemu2502

Permission is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the Software 
 without restriction, including without limitation the rights to use, copy, modify, 
 merge, publish, distribute, sublicense, and/or sell copies of the Software, and to 
 permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, 
INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A 
PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT 
HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR 
THE USE OR OTHER DEALINGS IN THE SOFTWARE.

### Conclusion

Thank you for exploring my React.jsPortfolio project! This project showcases my skills and experience with modern web development technologies, including React.js, Docker, and CI/CD pipelines. By providing a clear structure and comprehensive documentation, I aim to make it easy for others to understand, use, and contribute to the project.

Whether you are setting up your own environment, contributing through pull requests, or deploying the project to Docker Hub, I hope you find this project useful and inspiring. Your feedback and contributions are highly valued and can help improve this project further.

Feel free to connect with me through the provided social media links for any questions, suggestions, or collaboration opportunities.
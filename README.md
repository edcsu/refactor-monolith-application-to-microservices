# Refactor Monolith to Microservices

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![LinkedIn][linkedin-shield]][linkedin-url]

<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#contact">Contact</a></li>
    <li><a href="#acknowledgements">Acknowledgements</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

The project application, Udagram - an Image Filtering application, allows users to register and log into a web client, post photos to the feed, and process photos using an image filtering microservice. It has two components:

 1. Frontend - Angular web application built with Ionic framework
 2. Feed backend RESTful API - Node-Express application to get photos.
 3. Auth backend RESTful API - Node-Express application for authentication.

In this project you can also:

* Set up each microservice to be run in its own Docker container
* Set up a Travis CI pipeline to push images to Dockerhub
* Deploy the Dockerhub images to the Kubernetes cluster
* A reverse proxy server is added to add an extra layer of protection to the application

<!-- GETTING STARTED -->
## Getting Started

This is an example of how you may give instructions on setting up your project locally.
To get a local copy up and running follow these simple example steps.

### Prerequisites

* Install [Git](https://git-scm.com/downloads) for your Mac/Linux/Windows. Git is used to interface with GitHub.
* PostgreSQL client, the psql command line utility, installed locally. Using PostgreSQL involves a server and a client.
  The server hosts the database while the client interfaces with it to execute queries. Because we will be creating our server on AWS, we will only need to install a client for our local setup. The easiest way to set this up is with the [PostgreSQL Installer](https://www.postgresql.org/download/). This installer installs a PostgreSQL client in the form of the psql command-line utility. You can see the complete (server and client) installation instructions for Mac, Linux, and Windows.
* [NodeJS](https://nodejs.org/en/download/) v12.14 or greater up to v14.15 - Node.js is used to run JavaScript-based applications and NPM is a package manager used to handle dependencies. NodeJS installer will install both Node.js and npm on your system. Verify the installation using the commands:

  ```sh
  # v12.14 or greater up to v14.15
  node -v
  # v7.19 or greater
  npm -v
  ```

* [Ionic command-line utility v6](https://ionicframework.com/docs/intro/cli) framework to build and run the frontend        application locally. In general, Ionic Framework is used to make cross-platform applications using JavaScript. Verify the installation as:

  ```sh
  # v6.0 or higher
  ionic --version
  ```

* [Docker](https://docs.docker.com/desktop/#download-and-install) Desktop for running the project locally in a multi-container environment.

* AWS CLI v2 for interacting with AWS services via your terminal. After installing the AWS CLI, you will also have to configure the access profile locally.

  * Create an IAM user with Admin privileges on the AWS web console. Copy its Access key.
  * Configure the access profile locally using the Access key generated above:

    ```sh
    aws configure
    ```

* [Kubectl](https://kubernetes.io/docs/tasks/tools/#kubectl) command-line utility to communicate with Kubernetes clusters

### Installation

1. Clone the repo

   ```sh
   git clone https://github.com/edcsu/project.git
   ```

2. Cd into each of the respective projects to install their respective dependencies.

   ```sh
   npm install
   ```

<!-- CONTACT -->
## Contact

Your Name - [@your_twitter](https://twitter.com/skeith696)

Project Link: [https://github.com/edcsu/project](https://github.com/edcsu/project)

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/othneildrew/Best-README-Template.svg?style=for-the-badge
[contributors-url]: https://github.com/edcsu/project/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/othneildrew/Best-README-Template.svg?style=for-the-badge
[forks-url]: https://github.com/edcsu/project/network/members
[stars-shield]: https://img.shields.io/github/stars/othneildrew/Best-README-Template.svg?style=for-the-badge
[stars-url]: https://github.com/edcsu/project/stargazers
[issues-shield]: https://img.shields.io/github/issues/othneildrew/Best-README-Template.svg?style=for-the-badge
[issues-url]: https://github.com/edcsu/project/issues
[license-shield]: https://img.shields.io/github/license/othneildrew/Best-README-Template.svg?style=for-the-badge
[license-url]: https://github.com/edcsu/project/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://www.linkedin.com/in/ssewannonda-keith-edwin-443303129

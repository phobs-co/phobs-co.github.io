# REPPORT 
[![ci-badge](https://github.com/phobs-co/repport/actions/workflows/ci.yml/badge.svg)](https://github.com/phobs-co/repport/actions/workflows/ci.yml)

### Report Debris, Support Hawai’i!

# Overview

## About Us
Aloha! We are PHOBS, and we are excited to introduce our innovative solution to address the marine debris problem in Hawai’i. Our REPPORT App is designed to streamline and enhance the communication and coordination among various organizations involved in marine debris removal. We aim to create a centralized database and dispatch system that not only promotes efficient debris removal but also offers a platform for locals to report debris incidents. The ultimate goal of the REPPORT App is to significantly contribute to the preservation of Hawai'i's natural beauty and marine ecosystems.

<div style="display: flex;">
    <img src="doc/screenshots/repport-image1.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/repport-image2.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/repport-image3.png" style="max-width: 33%; padding: 10px;">
</div>


## Project Goals
The REPPORT App is designed with the following key goals in mind:

1. **Centralized Database:** Create a comprehensive centralized database that serves as the foundation for our system. This database will be accessible to the public in real-time, providing a wealth of valuable information about marine debris management.

2. **Real-time Public Access:** Develop user-friendly features that allow the public to access real-time information about ongoing debris removal efforts, locations, and progress.

3. **Dispatch Communication Tools:** Implement effective communication tools that enable seamless collaboration and coordination among various organizations involved in debris removal. This includes features for instant communication, updates, and task allocation.

4. **Comprehensive Data Capture:** Establish a cradle-to-grave database that captures data at all seven critical steps of marine debris management. This includes detecting debris in the ocean, removal efforts, debris type assessments, and disposal/recycling choices.

5. **Debris Amount and Proportion Reporting:** Enable the database to generate reports on debris amounts and proportions based on mapped locations, over time, and the efficiency of removal efforts. This data will help in assessing the impact of various initiatives.

6. **Debris Type and Polymer Type Tracking:** Implement features that categorize and track debris types and polymer types, helping organizations make informed decisions regarding the most effective removal and disposal methods.

7. **Disposal Mechanism Data:** Collect and analyze data related to the disposal mechanisms used for removed debris, including recycling options. This will promote environmentally responsible practices.

**The REPPORT App seeks to bridge the gap in communication, data collection, and transparency in marine debris management in Hawai'i. By achieving these goals, we aim to empower local communities, organizations, and government agencies to work together efficiently, leading to cleaner oceans and a brighter future for Hawai'i's natural environment.**

Together, let's report debris and support Hawai'i!

## Team contract:
[Team Contract](https://docs.google.com/document/d/1hqwtUSlLyOAMSRyKHdL3C6uYKi89OWbeOxxnrKbckJA/edit?usp=sharing)

## Milestone 1
[Milestone 1](https://github.com/orgs/phobs-co/projects/1)
<div style="display: flex;">
    <img src="doc/screenshots/login.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/map.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/registerorg.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/report.png" style="max-width: 33%; padding: 10px;">
</div>

## Milestone 2
[Milestone 2](https://github.com/orgs/phobs-co/projects/2)
<div style="display: flex;">
    <img src="doc/screenshots/editOrgProfile.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/reportedUnclaimedPage.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/registerorg.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/claimedPage.png" style="max-width: 33%; padding: 10px;">
    <img src="doc/screenshots/storedPage.png" style="max-width: 33%; padding: 10px;">
</div>

## Milestone 3
[Milestone 3](https://github.com/orgs/phobs-co/projects/3)


# User Guide

<!-- Maybe we can use the screenshots above? -->

# Community Feedback

# Developer Guide
This guide will lead you through the process of downloading, installing, running, and modifying the system for our GitHub public repository.

## Downloading The Repository
1. Start by navigating to the repository on the GitHub website.
2. Click on the green 'Code' button near the top right of the repository page.
3. To clone the repository using HTTPS, under "Clone with HTTPS", click the clipboard.
4. Open Terminal.
5. Change the current working directory to the location where you want the cloned directory.
6. Type `git clone`, and then paste the URL you copied earlier.
```bash
$ git clone https://github.com/phobs-co/repport
```

## Application Structure: Meteor.js (MongoDB & JSX) Application 

1. **Meteor Setup**: Meteor is installed globally on your machine. You initialize a new Meteor project using the CLI command `meteor create <app-name>`. This sets up the basic structure of your project, including Meteor, Node.js, and MongoDB.

2. **Project Structure**: A typical Meteor project has three main directories: `/client` (frontend code), `/server` (backend code), and `/both` (code run on both sides). 

3. **Database (MongoDB)**: MongoDB, Meteor's default database, automatically sets up during project initialization. Collections, set up in the `/both` section, can be observed by both server and client.

4. **JSX**: With the `react-meteor-data` package, Meteor supports JSX right out of the box. You can write your components using JSX in the `/client` folder.

5. **Client**: This includes `main.html`, `main.js`, and `main.css` files for HTML, JS, and CSS respectively. Here, you use Meteor's `react-meteor-data` package to create React components.

6. **Server**: Also contains a `main.js` file, which is the server's entry point. Here, you can publish your MongoDB collections to the client and setup server-side methods.

7. **Data Loading**: Meteor's data on the wire approach delivers data to the client as needed, via 'publications' (server side) and 'subscriptions' (client side).

8. **Real-Time Updates**: With its Distributed Data Protocol (DDP), Meteor provides real-time updates between the server (database changes) and client. It has a built-in pub-sub model for easy setup.

9. **Building & Running**: You can start your app using `meteor`, which also sets up hot code push and watches for source file changes. On building, Meteor bundles up your JavaScript, CSS, and HTML into minified JavaScript and starts a Node.js server.

Remember, this overview can vary based on actual set-up or project requirements. 

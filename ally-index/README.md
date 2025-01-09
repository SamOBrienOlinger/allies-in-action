<!-- # 24/7-hackathonteam-team9

View the live website [here](https://declan444.github.io/24-7-hackathon-team9/).

![image](https://github.com/user-attachments/assets/073b1221-62d8-45d6-94cf-87dfaa3775d9)

# Contents

- [Overview](#Overview)
- [User Experience UX](#UX)
- [Features](#features)
- [Technologies Used](#TechnologiesUsed)
- [Testing](#Testing)
- [Deployment](#Deployment)
- [Credits](#Credits)
- [Acknowledgements](#Acknowledgements)

# Overview

Know Yellowknife is positioned to be a central hub of information to dispel myths surrounding certain identities under the LGTBQ+ umbrella, build trust, familiarity and confidence between members of those identities and CIS gendered individuals. The focus is on building a bridge, support and understanding.

Additionally, a mini quiz will be accessible to help reinforce what has been learnt through the website and gamify the experience to encourage the user to come back and improve their score by developing their understanding of the LGBTQ community.

# User Experience

## Design

### First Time Visitor Goals

As a first-time visitor I want...

- to immediately understand the basic concept and purpose of the website
- to be able to intuitive understand the navigational instruments accessible on the website
- easily discover prominent features of the website
- to be able to view the device without issue regardless of my screen size
- to be able to easily take a quiz to test my knowledge and learn about the LGBT community
- easily understand how the quiz works
- track my progress during the quiz and see what question I am on
- receive continuous feedback on my score during the quiz

### Returning Visitor Goals

As a returning visitor I want...

- To be able to easily locate information I had previously accessed
- To easily contact the site owner
- reattempt the quiz in order to try and obtain a higher score
- To try and beat my previous high score in the quiz

### Frquesnt Visitor Goals

### Colour Scheme

We will be designing our site with soft pastel colours closely matching those found on the Pride flag in order to pay homage to the various LGBTQ communities. Where necessary the colours white and black will also be used in order to create optimal contrast between text and backgrounds for accessibility purposes.

![Colour Scheme](assets/documentation/img/color-palette.png)

### Typography

For typography across the site, we will be using a combination of "Lilita One" and "Montserrat". Both fonts are provided by Google Fonts. Lilita One is a bold and impactful font which will be used for things like section headings, links and buttons whereas Montserrat is a beautiful yet simplistic font in its own right with wonderful readability at smaller font sizes. Therefore, Montserrat will be used for the main text across the website pages.

### Imagery

Imagery for the website will consist of images paying tribute to the bravery and bold personality of members of the various LGBTQ communities as well as some imagery from historical moments and places, for example, Stonewall. Where possible the images will be sourced from Unsplash which provides images that are free to use. Where necessary we will use images from other sites with attribution.

### Wireframes

#### Home

[home](https://github.com/user-attachments/assets/3cd395fb-7281-4ba3-92ce-e6e6c51e78ed)

#### Quiz

[quiz](https://github.com/user-attachments/assets/03041377-ea70-4283-b65b-77dd496c4f50)

#### About

[about](https://github.com/user-attachments/assets/88666e63-2622-4d01-a83c-fd7362d005f6)

#### Learn

[learn](https://github.com/user-attachments/assets/f7291377-2b0c-4866-b2fb-6412c40cc9e8)

#### Contact

[contact](https://github.com/user-attachments/assets/f418da93-5a1d-4245-9199-1f0f055a31d9)

# Features

- Responsive Mobile-First design approach ensuring that the website displays appropriately across all device types
- Appropriately themed visual fidelity to ensure appeal and engagement
- A comprehensive source of information on a broad range of identities
- A replayable quiz

## Home Page

The home page serves as a way to let the user know what the site is for, the ethos and purpose. The user is
greeted with an attention grabbing carousel of lgbt+ images and a call to action to take part in the quiz.
Further down the homepage, the user can see basic information about what the site hopes to achieve.

## Learn Page

From here the user can browse through the available lgbt+ resources. There is a comprehensive terminology list,
as well as an overview of lgbt+ history. Each section can be viewed by clicking the heading to view a dropdown
of information.

## Quiz Page

The quiz page is where the user can take part in the lgbt+ quiz and test their knowledge. Local high scores are
saved to the users device, so they can come back and try again. The user is asked 10 questions from a pool of
20+ questions, so the quiz is different each time you take part.

## About Page

The about page shows who the developers were for the hackathon/project team. The user can view the info cards
and find links to the developers social and Github pages.

## Contact Page

On the contact page the user can submit a simple form to get in contact with the team.

# Technologies Used

## Languages Used

- HTML
- CSS
- JavaScript

## Frameworks, Libraries and Programmes used

- [Bootstrap](https://getbootstrap.com/)
- [Fontawesome](https://kit.fontawesome)

# Testing

## Bug &amp; Solutions

### Solved Bugs

- We had an issue with the quiz sometimes repeating questions. The initial implementation used an array that was prepopulated with the ID of each question. An algorithm would generate a random number and get the ID from the array at the index of the random number, then prompt the user with the question associated with that ID. This implementation was deemed to be convoluted and, as mentioned, had a bug causing the same questions to be asked multiple times on occasions. Rather than investigate the issue to find the cause we opted to simply rework the algorithm. This was due to time constraints and the fact that we conceptualisied a much simpler solution. Now, when a question is asked it adds the question ID to a separate array, which is checked to see if the array already contains that ID, if it does, it simply generates a new number and checks that the associated question ID isn't already in the list. This is still not perfect but is good enough in this scenario.

- Our video background was initially picked up as having errors because it was defined as a section and had no headings within it. In order to resolve this, we changed the parent HTML element to be a simple `div` instead of a `section`.

### Known Issues

## Validation Results

### W3C HTML Checks

While all pages have some messages rated as "info" we have decided to ignore them as they will have little to no impact on usability or accessibility and within the scope of this project, we would rather use the time elsewhere. For the sake of this project, we are prioritising "warning" and "error" messages.

[Index](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdeclan444.github.io%2F24-7-hackathon-team9%2Findex.html)

[Quiz](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdeclan444.github.io%2F24-7-hackathon-team9%2Fquiz.html)

[About](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdeclan444.github.io%2F24-7-hackathon-team9%2Fabout.html)

[Learn](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdeclan444.github.io%2F24-7-hackathon-team9%2Flearn.html)

[Contact](https://validator.w3.org/nu/?doc=https%3A%2F%2Fdeclan444.github.io%2F24-7-hackathon-team9%2Fcontact.html)

We have a single warning for the use of an inline styling including a CSS variable. This is only a minor concern. The inline CSS variable is implemented to avoid unecassary Javascript so this is a compromise we have discussed and are willing to make. Other than this we have no reported warnings or errors.

### W3C CSS Checks

[CSS](http://jigsaw.w3.org/css-validator/validator?lang=en&profile=css3svg&uri=https%3A%2F%2Fdeclan444.github.io%2F24-7-hackathon-team9%2F&usermedium=all&vextwarning=&warning=1)

The website successfully passes the W3C CSS Validation checks.

### JSHint

In order to verify our JavaScript file does not have any errors we have validated the app.js file using JSHint. The results are visible in the image below. No errors were found.

![JSHint Image](assets/documentation/img/js-hint.png)

### Lighthouse Report

Lighthouse testing has been thoroughly conducted on every page of the website, with each page excelling in all areas. Particularly noteworthy is the perfect accessibility score of 100 on every page!

Homepage

![lighthouse_testing_home](assets/documentation/img/lighthouse_testing_home.png)

Quiz

![lighthouse_testing_quiz](assets/documentation/img/lighthouse_testing_quiz.png)

About

![lighthouse_testing_about](assets/documentation/img/lighthouse_testing_about.png)

Learn

![lighthouse_testing_learn](assets/documentation/img/lighthouse_testing_learn.png)

Contact

![Lighthouse_testing_contact](assets/documentation/img/lighthouse_testing_contact.png)

### a11y Report

We used a11y to check the site for any contrast issues. The report can be seen in the image below. There were no accessibility issues found.

![a11y Contrast Test Result](assets/documentation/img/contrast-check.png)

### Responsiveness Testing

The site has been tested on all screen sizes and performs as expected.

### Manual Testing

Manual testing can be found in the [Testing File](TESTING.md)

Testing specifically for the Quiz can be foound in the [Quiz testing File](QUIZ-TESTING.md)

# Deployment

## Local Testing

- The project was deployed to Github Pages using the following steps:

  - Create and/or Log in to GitHub
  - Locate the repository within GitHub
  - Within the repository, click on Settings
  - Within the settings page locate the sub-menu on the left hand side and click on Pages
  - Under "Source" select "Branch:main" then /root
  - Click Save
  - Wait a few moments for the repository to deploy
  - At this point the repository will be deployed and ready to view

## Cloning the Repository

- Follow the steps below to clone the repository:

  - Locate the repository
  - Click the button labelled "Code" to the top right of the screen
  - Click HTTPS and copy the link provided
  - In your local environment navigate to the desired directory
  - Open a terminal and type "git clone `repository-url`"
  - Press enter to begin the cloning process

  ## Forking the Repository

- Follow these steps to fork the repository

  - Locate the repository on GitHub
  - Click `Fork` in the top right corner
  - If necassary, select the owner for the forked code under the `Owner` dropdown menu.
  - Optionally, edit the `Repository Name` field to rename your forked repository
  - Optionally, use the `Description` field to input a description of your fork
  - Select "Copy the DEFAULT branch only"
    - This is another optional step, many scenarios only require a fork of the default branch. If you do not select this you will copy all branches into your fork
  - Click `Create Fork`

# Credits

## Code

- [Josh's CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/)
- [Google Fonts](https://fonts.google.com)
- [SweetAlert](https://sweetalert2.github.io/)
- [JQuery](https://ajax.googleapis.com)

## Images

- [Unsplash](https://unsplash.com/) - For imagery used across the site

## Videos

- [Pexels](https://videos/pexels.com) - For video used on the home page

## Content

- [Stonewall](https://www.stonewall.org.uk/list-lgbtq-terms) - For a list of terminology and their explainations

## Programs

- [CloudConvert](https://cloudconvert.com/) - For editing and optimizing images

# Acknowledgements

- Many thanks to the 'Hackteam' who give their time and energy voluntarily to support Code Institute's July 2024 Hackathon.

  ![Hackathon Team](assets/img/README.me-image-hackteam.png) -->

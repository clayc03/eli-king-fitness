# ELI KING FITNESS
## Introduction

Eli King Fitness is a website of a personal trainer advertising his services in Almere, Netherlands. Eli King Fitness offers personal training classes and also group classes for Beginners and Advanced fitness enthusiasts.

Users of this website will be able to learn more about the founder himself Eli King, the group class schedules and time slots for personal training sessions. The website will also provide information of the different prices for each group class and private session, contact details and where the gym is located.

![Mockup screenshot](/assets/images/cover-page-readme.png)

## [View life website in github pages](https://clayc03.github.io/eli-king-fitness/) 

<u>*Disclaimer - This website is for educational purpose only*</u>
<hr>

## **[Table of Contents](#contents)**
1. **[Features](#features)**
This website consists of five pages, four of these pages are accessible from the navigation menu.
The last page is linked to the contact form and is a submission confirmation page.

Below are the website features:

## Navigation bar

* The Navigation bar is consistant on each page:

    * The logo is on the left side, clicking on the logo will navigate the user back to the home   pageas.
    * The menu list on the right side consists of four links to each page:
        * Home
        * Meet Eli
        * Plans & Pricing
        * Get in Touch

## Home page - About Section

* The About section is on the homepage and gives information about the different classes be offered at Eli King Fitness and also a brief description about the facility where these classes take place. Also on the homepage is the address and a google map for address reference.

## Meet Eli

* This page gives information about the founder Eli King and his experience and qualifications obtained.

## Prices & Plans

* This page gives the user information on the different prices for each class (Beginner or Advanced) and private session as well as the schedule for each.

## Get in Touch

* This page the user can complete to get in contact with Eli King Fitness and for a response on any query or information required. This page is linked to a confirmation page that the users message was send successfully.

## Footer

* The Footer is consistent on each page. The Footer has links to social media websites, these links open in a seperate tab in a browser.

[Back to Table of contents](#table-of-contents)

2. **[Testing](#testing)**

## Functionality testing 

 I used Mozilla web developer tools and Chrome developer tools throughout the project for testing and solving problems with responsiveness and style issues.
 
 [Unicorn Revealer](https://chrome.google.com/webstore/detail/unicorn-revealer/lmlkphhdlngaicolpmaakfmhplagoaln?hl=en-GB) extension to chrome browser was very helpful.


## Compatibility testing
 Site was tested across multiple virtual mobile devices and browsers. I checked all supported devices in both Mozilla web developer tolls and Chrome developer tools. 
 
 I tested on hardware devices such as: Lenovo ideapad with Ubuntu and Windows OS's, Lenovo smartphone with Android 7, Google pixel 3 with Android 11.


## User stories testing

### As a business owner:

- I would like to present myself and my offer on the website clearly to potential customers.
    > Name, photo of the instructor and top skills are on each page in portfolio section. Career path section at home page provides more details.

- I need to make sure that my current and new customers will find a professional help with their diets, personal or group trainings.
    > Customers can achieve this by contacting through contact form. They can choose interesting topic and describe their needs in a message box.

- I want my customers to be able to learn how to use my website intuitively and easily.
    > Each site has a fixed navigation menu and is accessible at all times. All content is presented with minimalistic approach.

- I would like to build and maintain relationship with potential and current customers.
    > Customers are able to find a links to social channels at the bottom of each page. Alternatively they can contact by email or contact form.


### As a new customer:
- wish to find information about personal trainer and check her/his qualifications.
    > User can see essential description on the home page. More information can be find in about page.

- I would like to contact with a diet coach to change my eating habits and start healthy lifestyle.
    > User can find a contact form in contact page. Alternatively can use an email. Email address if located in a footer the bottom of each page.

- I want to join in a fitness group with professional trainer, to find motivation and spend time actively.
    > Brief class description of fitness group classes can be find on the home page below career path section. Offer site provides more detailed description. Frome there user can click contact us button and send a message to the traier.

### As a returning customer:
- I need to contact my diet coach to reschedule my meeting.
    > User can find a contact form in contact page. Alternatively can use social channels or email.

- I would like to check timetable for current days and times for a group trainings.
    > Each site has time table at the bottom of the page.

- I want to show my friend a location of the fitness studio where we can join for a semi private personal training.
    > Each page contains location information in a footer. Users are able to find a location map in contact page.


---
## Issues found during site development

* #### Horizontal scrolling bar on the bottom of the screen.
![testing_issue_1](testing/testing_issue_1.png)

I used [grid markup](https://getbootstrap.com/docs/4.5/components/card/#header-and-footer)
to create two sepereate collumns. To achieve this I had to use *.row* in first *div* element and *.col-sm-6* in the second *div* element.
After that I found that horizontal scrolling bar appear on the bottom of the screen.
Using mozilla developer tools I noticed that by default class *.row* has *margin-right: -15px;* and *margin-left: -15px;*

To fix this I created new class *.no-row-margin* and set both margins to 0px.

> After I gain more experience with bootstrap I found that I could achive this by [no-gutters](https://getbootstrap.com/docs/4.0/layout/grid/#no-gutters) class.

> I read bootstrap documentation about [Spacing](https://getbootstrap.com/docs/4.0/utilities/spacing/) and I decided to use predefined classes for paddings and margins in the project.
By doing this I think my code looks cleaner and will be easier to understand by other developers.


* #### Ipad screen compatibility

I found a bugs on Ipad screens. I would like to keep years dates just above the stars, but they were shifted.

![testing_issue_2](testing/testing_ipad_screen.png)

I had to create a block element with a class "ipad-screen" and non-breaking space element inside a block element.
In CSS file I had to create @media rule that will show this block element on Ipad displays only.

>}
@media screen and (max-width: 991px) and (min-width: 0px),(min-width:1200px){
    .ipad-screen {
    display: none;
}
}

![bug_solutino1](testing/bug_solution1.png)

![bug_solutino2](testing/bug_solution2.png)

## Performance testing

I run [Lighthouse](https://developers.google.com/web/tools/lighthouse/) tool to check performance of the website.
I had to do couple of changes to improve performance. Screenshots are presented below:

![bug_performance1](testing/performance1.png)
![bug_performance2](testing/performance2.png)

Final results:
![performance_final](testing/performance_final.png)
I noticed that this tests scores vary from time to time and depends on external libraries as well. 


3. **[Technology](#technology)**
4. **[Unfixed Bugs](#unfixed-bugs)**
5. **[Deployment](#deployment)**
6. **[Credits](#credits)**
7. **[Screenshots](#screenshots)**




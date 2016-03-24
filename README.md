# Project Overview

In this project, Udacity provided a web-based application that reads RSS feeds. It has Jasmine included and I completed the tests that were originally TODOs and added an additional test for future functionality. The original project is at http://github.com/udacity/frontend-nanodegree-feedreader and it is a part of Udacity's [Front-end Web Developer Nanodegree](https://www.udacity.com/course/front-end-web-developer-nanodegree--nd001)

## Viewing the Project 
### View the Project Online
You can view the project results online at http://kellim.github.io/feed-reader-testing

### Download the project
* Click the `Download Zip` button to download the project. 
* Open `index.html` which currently has Jasmine included at the bottom for convenience. 

Note: As mentioned below, all the tests pass except the last 2 which are for functionality that is not implemented yet. 

## About the Tests

The tests I wrote live in the Jasmine Spec file at */jasmine/spec/feedreader.js*.
Tests were created for the TODOs to:
* Loop through each feed in the allFeeds object and ensure it has a URL defined and that the URL is not empty.
* Loop through each feed in the allFeeds object and ensure it has a name defined and that the name is not empty.
* Ensure the menu element is hidden by default.
* Ensure the menu changes visibility when the menu icon is clicked. This test has two expectations: does the menu display when clicked and does it hide when clicked again.
* Ensure when the loadFeed function is called and completes its work, there is at least a single .entry element within the .feed container. Note: *loadFeed() is asynchronous so this test and the next one use Jasmine's beforeEach and asynchronous done() function.*
* Ensure when a new feed is loaded by the asynchronous loadFeed function that the content actually changes.

I created an additional Test Suite called 'Site Color' with two tests to ensure that when a visitor clicks a link to change the site background color to purple that it acutally updates the sliding sidebar menu and the header with the css to change the background color to the new purple color. These are the only 2 tests that will currently fail because the site does not have the functionality to change background color yet. The test failures are intended because in test-driven development, you write the tests first, they fail, and then you update your code so they pass the tests.

## Resources

* [JavaScript Testing Course (Udacity.com)](https://www.udacity.com/course/javascript-testing--ud549)
* [Jasmine Documentation (GitHub)](http://jasmine.github.io/)
* [JavaScript Testing with Jasmine Video Tutorials (YouTube)](https://www.youtube.com/playlist?list=PLOxOmO43E6Jt0SruKGxtZs-W3PJN90G_a)
* [JavaScript Koans](https://github.com/mrdavidlaing/javascript-koans) - the Koans use Jasmine to teach JavaScript concepts and are good Jasmine Practice. They go through some of the Koans in the JavaScript Testing with Jasmine Video Tutorials on YouTube.
* [Sublime Jasmine(GitHub)](https://github.com/NicoSantangelo/sublime-jasmine)
* [jasmine-jquery (GitHub)](https://github.com/velesin/jasmine-jquery)
* [Testing DOM Events Using jQuery and Jasmine 2.0 (htmlgoodies.com)](http://www.htmlgoodies.com/beyond/javascript/js-ref/testing-dom-events-using-jquery-and-jasmine-2.0.html)

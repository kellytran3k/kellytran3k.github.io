---
layout: page
title: just renegade
permalink: projects/just-renegade/
subtitle: Just Renegade
---

# You've heard of Tik Tok right?

**and I'm assuming you've played Just Dance at least once in your life.**

Well, this is the best of both worlds!

The '*Renegade*' was a popular dance trend on social-media platform '*Tik Tok*' in 2020.
The popular choreography had over **300,000 people** dancing to it, and had a huge following of celebrities like *Kourney Kardashian*, *Bella Thorne*, and *Noah Schnapp* participating.

My hackathon team and I incorporated the '*Just Dance*' game concept which gave players a score based on how accurated they did the movements of the dance.

/**Just Renegade was a submission for UGAHacks 5**/

![](/assets/img/just-renegade.png)

## Application:

We developed a pseudo native app using Python and front-end web technologies. Users interact with a Selenium-controlled Chrome browser, which changes the text in an invisible paragraph tag to communicate with a Python script. This script controls the state of the game and even edits the DOM to display the video.

We used the OpenPose library to detect poses, and using some clever math involving calculating angles between points of interest, we compared the user's video to the original video to score their accuracy.

A result video with a skeleton tracking overlay is generated in addition to tons of json output data, upon which we conducted data analysis with Python scripts. All of this is then loaded with a Bootstrap/JQuery frontend and displayed as a webpage for the end user.

## Built With:

- **OpenPose** - Real-time multi-person keypoint detection library for body, face, hands, and foot estimation created and maintained by members of Carnegie Mellon University

- **Selenium** - a portable framework for testing web applications; provides a playback tool for authoring functional tests without the need to learn a test scripting language

- **NumPy** - a library for the Python programming language, adding support for large, multi-dimensional arrays and matrices, along with a large collection of high-level mathematical functions

- **Bootstrap** - an open source toolkit for developing with HTML, CSS, and JS

- **JQuery** - a JavaScript library designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax

- **TikTok** - a video-sharing social networking service used to create short lip-sync, comedy, and talent videos

## Takeaway
I mainly worked on JQuery frontend design. It was a great learning experience for me, and loads of fun. Probably the best hackathon I've been to yet!

### Special thanks and shoutout to the best and funnest team ever:
*Kavin Phan, Richard Red, Sarah Yoo*

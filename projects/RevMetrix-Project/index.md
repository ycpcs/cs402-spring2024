---
layout: default
course_number: CS402
title: CS Capstone II (RevMetrix Project)
---

--- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- ---

## CS402: CS Capstone II (RevMetrix Project)

## Spring 2024

--- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- ---

This is the web page for the RevMetrix Project for CS402 Spring 2024 at [York College of Pennsylvania](http://www.ycp.edu).  All information specifically related to the RevMetrix Project will be posted here.

## Links

* [CS402-Fa24 Website](../../index.html)
* [Syllabus](../../syllabus.html)
* [Schedule](schedule.html)
* [RevMetrix Project Wiki](https://docs.revmetrix.io)
* [RevMetrix Research](https://research.revmetrix.io)

## RevMetrix Project Description

You will be continuing development of the RevMetrix Project, building upon the initial accomplishments from the [RevMetrix Project Capstone I (CS400) Team from Fall 2023](https://ycpcs.github.io/cs400-fall2023/projects/RevMetrix-Project).

Your basic goals for the semester are to:

*	Develop a functional RevMetrix **Bowler** User Interface (RMxB-UI) that allows for bowler input to be collected, stored, retrieved, and displayed, utilizing the RevMetrix User Back-End Database (RMxB-DB). The RMxB-UI is a multi-platform phone application.  If the cross-platform development tools support it, a Windows PC version of the RMxB-UI application would also be useful (but not a high priority).  Here is the description for the [RevMetrix Bowler UI Requirements](RevMetrix.html).  It does **NOT** cover the Research User Interface.  And here is a [Prototype Shot Entry Page](RevMetrix-Bowler-UI-Shot-Entry.html) to give you a basic idea of user workflow and functionality.  This is a prototype.  It is, **by no means**, quality code, as it contains the first JS I've ever written - with a lot of help from ChatGPT.  It should however, give you an idea of how the user will enter the results for each shot.

*	Develop a similar functional RevMetrix **Research** User Interface (RmxR-UI) that allows for research data input to be collected, stored, retrieved, and displayed, utilizing the RevMetrix Research Back-End Database (RMxR-DB). The RMxR-UI will be a Windows laptop touchscreen application.  The data stored in the RMxR-DB will be a superset of the data stored in the RMxB-DB.

*	Continue development of the RevMetrix Back-End, including both databases (RMxB-UI and RMxR-UI).

*	Continue development and maintenance of the RevMetrix Wiki, including accurate and detailed instructions on how to set up all of the various development environments, and the various deployments to Digital Ocean.

*	Continue development on the Unity Simulator that is intended to generate animated ball paths that can be used to create known video frame and ball path data for use by Ciclopes.

*	Develop automated algorithms for frame-by-frame video processing of the Unity Simulation animation to extract the lane boundaries and ball locations within those boundaries.  Confirm the accuracy of the above algorithms by comparing their output with the Unity Simulation data that generated the frames for the animation.
real video and start to modify, as necessary.

*	Test the applicability of the above Ciclopes algorithms on real bowler video, using similar camera angles as were used on the Unity animations.

*	Develop algorithms that will extract relevant ball path and velocity data from the frame-by-frame analysis of the video, after transforming the lane boundaries and the ball location within each frame into a collection of normalized rectilinear frames.

*	Refine the Ciclopes algorithms above to work reliably with real bowler video.

*	Continue to develop BLE (Bluetooth Low-Energy) connectivity between BLE sensor hardware (3-axis accelerometer, 3-axis gyroscope, ambient light sensor) and a phone application so that the BLE sensor suite can upload live data to a phone application.


Here are links to the previous research that Professor Hake conducted as part of his Master's Theses:

*	[RevMetrix MEng ESci Thesis](Hake-MEngESci-Masters-Thesis.pdf)

*	[RevMetrix MEng ESci Final Presentation](Hake-MEngESci-Masters-Defense-Presentation.pdf)

Here is a set of raw data from an actual bowling session.  There are two versions:

*	A [text version](./resources/Shots(0-19)-Suburban(8-29-10).txt) that contains the EEPROM contents, as well as a CSV extraction of the raw data from those EEPROM contents.

*	An [Excel Spreadsheet](./resources/Shots(0-19)-Suburban(8-29-10).xlsx) that also contains graphs of the extracted raw data for each shot in the session.

Here is an an [Updated Excel Spreadsheet](./resources/Shots(0-19)-Suburban(8-29-10)-BallRecord00002-annotated.xlsx) that contains annotations explaining the various components of the raw data.  A second page has been added for Ball Record 00002 that contains the actual 32-bit RTC (Real Time Clock) time stamps for all of the ADXL Pages, the Light Pages, and the SmartDot Events to be sent to the phone application.  The SmartDot Event time stamps could be used to send event signals via BLE in real time (during simulation) from the SmartDot simulator to the phone application.  For Ball Record 00002, all of the individual ADXL and Light sample time stamps have been recalculated based on the actual RTC captures for each page.  You can use these RTC time stamps to generate the exact time stamp values captured in the raw data when running the simulator.  Please look in the **Notes** for the cells for additional information.  

## News
<!-- Commenting out YCPHacks-specific News until it's needed - and the dates could change, anyway

* 11-14-22: Assignment 7 (Final Report and Final Peer Evals) are both due by Noon, Sunday, 12-11-22

* 11-14-22: Assignment 7 (Final System Presentation) is from 11:00am to 12:50pm, Monday, 12-5-22, with presentation and demo in class

* 11-14-22: Assignment 7 (Draft Technical Report) is due by Noon, Sunday, 12-4-22, in your Google Team Drive

* 11-14-22: Your status report for Monday, 11-28-22 has been moved to Wednesday, 11-30-22

* 11-14-22: On Monday, 11-21-22, you will be giving your status update to your clients: Tyler Franks & David McHugh 

* 10-28-22: Assignment 6 (50% Working System) is at 11:00am, Monday, 11-14-22, with presentation and demo during class

* 9-29-22: Mid-Semester Peer Evals are due Wednesday, 10-26-22 by Noon, via email in PDF form

* 9-29-22: Assignment 5 (Minimal Working System) is due 11:00am, Monday, 10-24-22, with presentation and demo during class

-->

* 2-18-24: Posted the basic requirements for the RevMetrix Project for this semester.

* 2-16-24: Posted a link to a JavaScript prototype of the Shot Entry Page to give you a basic idea of user workflow and functionality.  This is a prototype.  It is, **by no means**, quality code, as it contains the first JS I've ever written - with a lot of help from ChatGPT.  It should however, give you an idea of how the user will enter the results for each shot.

* 2-16-24: Posted a link to the RevMetrix Bowler User Interface Requirements.

* 2-5-24: [Assign03: Detailed Project Proposal Design and Schedule](../../assign/assign03.html) is due before class (with presentation in class) on Monday, 2-19-24.

* 1-26-24: [Assign01: Individual Proposal and Wish List](../../assign/assign01.html) is due before class (with presentation in class) on Monday, 2-5-24.

* 1-26-24: Links for Professor Hake's RevMetrix research (both MEng ESci thesis and Final Presentation) have been posted above.  We will discuss which sections are directly relevant for this semester's work.

[General CS400 Fall 2023 News](../../index.html)
---
layout: default
course_number: CS402
title: CS Capstone II (RevMetrix Project)
---

--- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- ---

## CS400: CS Capstone I (RevMetrix Project)

## Fall 2023

--- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- --- ---

This is the web page for the RevMetrix Project for CS 400 Fall 2023 at [York College of Pennsylvania](http://www.ycp.edu).  All information specifically related to the RevMetrix Project will be posted here.

## Links

* [CS400-Fa23 Website](../../index.html)
* [Syllabus](../../syllabus.html)
* [Schedule](schedule.html)
* [Prototype Shot Entry Page](RevMetrix-Bowler-UI-Shot-Entry.html)
* [RevMetrix Bowler UI Requirements](RevMetrix.html)


## RevMetrix Project Description
Here are links to the previous research that Professor Hake conducted as part of his Master's Theses.

[RevMetrix MEng ESci Thesis](Hake-MEngESci-Masters-Thesis.pdf)

[RevMetrix MEng ESci Final Presentation](Hake-MEngESci-Masters-Defense-Presentation.pdf)

Here is a set of raw data from an actual bowling session.  There are two versions:

1) A [text version](./resources/Shots(0-19)-Suburban(8-29-10).txt) that contains the EEPROM contents, as well as a CSV extraction of the raw data from those EEPROM contents.

2) An [Excel Spreadsheet](./resources/Shots(0-19)-Suburban(8-29-10).xlsx) that also contains graphs of the extracted raw data for each shot in the session.

3) An [Updated Excel Spreadsheet](./resources/Shots(0-19)-Suburban(8-29-10)-BallRecord00002-annotated.xlsx) that contains annotation explaining the various components of the raw data.  A second page has been added for Ball Record 00002 that contains the actual 32-bit RTC (Real Time Clock) time stamps for all of the ADXL Pages, the Light Pages, and the SmartDot Events to be sent to the phone application.  The SmartDot Event time stamps can be used to send event signals via BLE in real time (during simulation) from the SmartDot simulator to the phone application.  For Ball Record 00002, all of the individual ADXL and Light sample time stamps have been recalculated based on the actual RTC captures for each page.  You can use these RTC time stamps to generate the exact time stamp values captured in the raw data when running the simulator.  Please look in the notes for the cells for additional information.  

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

* 9-29-22: Assignment 4 (Analysis & Design) has been moved to 11:00am, Wednesday, 10-5-22, with presentation during class

* 9-19-22: Assignment 3 (Requirements) is due by 11:00am, Monday, 9-26-22, with presentation during class

* 9-19-22: Assignment 2 (Weekly Journals) are now due every Monday by 11:00am (prior to class), with a summary presentation in class on the days that do not already have another assignment due

* 8-27-22: Assignment 1 (Readiness Demo) is due by 11:00am, Friday, 9-16-22, with presentation during class

* 8-27-22: Assignment 1 (Project Proposal) is due by 11:00am, Friday, 9-9-22, with presentation during class

-->

* 2-16-24: Posted a link to a JavaScript prototype of the Shot Entry Page to give you a basic idea of user workflow and functionality.  This is **by no means** quality code, as it contains the first JS I've ever written - with a lot of help from ChatGPT.  it should however, give you an idea of how the user will enter the results for each shot.

* 2-16-24: Posted a link to the RevMetrix Bowler User Interface Requirements.

* 2-5-24: [Assign03: Detailed Project Proposal Design and Schedule](../../assign/assign03.html) is due before class (with presentation in class) on Monday, 2-19-24.

* 1-26-24: [Assign01: Individual Proposal and Wish List](../../assign/assign01.html) is due before class (with presentation in class) on Monday, 2-5-24.

* 1-26-24: Links for Professor Hake's RevMetrix research (both MEng ESci thesis and Final Presentation) have been posted above.  We will discuss which sections are directly relevant for this semester's work.

[General CS400 Fall 2023 News](../../index.html)
---
layout: default
course_number: CS402 (RevMetrix)
title: "RevMetrix Bowler User Interface"
---

Project Summary
===============
The RevMetrix Bowler User Interface (UI) will allow bowlers to record and track their performance by providing the means for entering their scores at the [indivdual shot level](RevMetrix-Bowler-UI-Shot-Entry.html).  The UI will also keep score for the bowler as a Game and Session progress.  That will be the basic input side of the UI.

The output side of the UI will provide several functions:
-	The UI will provide the accumulated scores for bowling Sessions and will allow the user to interrogate the overall collection of stored Games across a wide range of queries.
- The UI will also provide access to statistics based on the individual Frames/Shots that the User recorded while bowling those Games. The user will be able to request a wide variety of statistics and graphs for not only their Game scores, but also the individual results for each Frame/Shot on a frame-by-frame and shot-by-shot basis, with correlations and trends between Frame/Shot statistics and Game scores.

Basic Requirements
==================
Here are the basic requirements for the RevMetrix Bowler User Interface.  Below are listed the major components for the UI, with descriptions, along with their sub-components.

The basic structure is Event->Session(s)->Game(s)->Frames->Shot(s).

**Event**: A bowler can participate in several types of **Events**: practice, leagues, tournaments.  The User will be able to register various Events through the UI.  Event information will include:

-	**Name:** the name of the Event
-	**Type:** practice, league, tournament
-	**Location(s) of the Event:** the bowling establishment(s) where the Event will occur
-	**Sessions:** a list of the Sessions associated with the Event
-	**Stats:** the overall average for the Event, the high and low Session and Game scores for the Event, 1st, 2nd, 3rd Game averages, etc...
-	**Standings**: where the User currently stands (or finished) in the rankings of the Event (if known)

**Session:** An Event is composed of one or more **Sessions**, i.e., a league generally meets weekly at a scheduled time, generally at the same establishment - although there are travelling leagues that bowl at different establishments each week.  Tournaments can have multiple Sessions in a single day and can span multiple days and even weeks across multiple establishments.  Session information will include:

-	**Establishment:** picked from the list for the Event
-	**Date:** date of the Session
-	**Time:** scheduled starting time of the Session
-	**Team Opponent:** for a team Session, the opponent's team name
-	**Individual Opponent:** for match play, the opponent's name (it is possible to have a team opponent and an individual opponent at the same time)
-	**Score:** total score for all Games in the Session
-	**Stats:** # of first Shots, # of strikes, spares, opens, splits, spares converted, splits converted, etc...
-	**Games:** a list of Games associated with the Session

**Game:** A Session consists of a number of **Games**.  For example, a league Session generally consists of 3 games each week, whereas a practice Session could consist of any number of Games (or even partial Games - just a series of Frames).  Game information will include:
-	**Lane(s):** the lane(s) on which a Game was bowled.  A Game can be bowled on multiple lanes.  For example, a league Session is generally conducted on an odd-even pair of lanes, alternating Frames between the two lanes.
-	**Game #:** the chronological order of the Game within the Session
-	**Score:** the score for the Game
-	**Starting Lane:** the lane the first Frame was bowled on
-	**Frames:** a list of Frames associated with the Game

A **Game** consists of 10 Frames. Frame information includes:
-	**Frame #:** the chronological order of the Frame within the Game
-	**Lane:** the lane the Frame was bowled on
-	**Result:** indicates the result for the Frame: strike, spare, open, etc...
-	**Shots:** a Frame can have up to three Shots (the first 9 have up to two Shots, the 10th can have up to three Shots

A **Shot** is the most basic component of a Game.  For the first 9 frames, a Frame consists of one or two Shots.  For the 10th Frame, there can be up to three Shots.  The Shot information consists of:
- 	**Shot #:** the chronological order of the Shot within the Frame
-	**Ball:** the Ball used for the Shot
-	**Count:** pins knocked down on the Shot
-	**Leave:** a list of the number of each pin that was left standing after the Shot
-	**Type:** the type of leave: strike (no pins standing), spare, open, split, washout, etc...


Other Components
================
-	**Account:** an account the User creates in order to enter and interact with their data
-	**Event Registration:** a means for the User to add Events to their Event Collection
-	**Ball Registration:** a means for the User to add Bowling Balls to their Bowling Ball Arsenal (bowling balls that they own/use)
-	**Ball:** an individual entry in the Ball Arsenal
-	**Establishment Registration:** a means for adding a bowling establishment to the collection of bowling establishments that host Events the bowler has/will bowl in.
-	**Establishment:** an individual entry in the Establishments collection



Basic Functionality
===================

## Bowling

-	The bowler will select an Event, Establishment, Session, Lane(s), Bowling Ball(s), and then commence to bowl.
-	The UI will automatically keep track of Game, score, lane, ball, Frame, and Shots.
-	The user will roll each Shot and enter the pins left standing via an [inverted equilateral triangle of numbered circles](RevMetrix-Bowler-UI-Shot-Entry.html), which represents the pin layout at the pin deck of a bowling lane).
-	Pin selection will be clickable and touch-sensitive for touch screens.
-	The User will select the pins that were left standing after each Shot.
-	The UI will update the count for the Shot as the user selects/deselects the pins left standing.
-	The User will be able to select 'X' if they rolled a strike, or '/' if they converted a spare.
-	The User will be able to select 'F' if they committed a foul, or '-' if they threw a gutterball, or missed all of the pins on a spare attempt.
-	After the User has finished their selection for a Shot, they will submit that Shot, which sends the Shot information to the RevMetrix System for analysis, storage, and processing.
-	The System will then respond and set up the next Shot and/or the next Fframe, while also displaying the current score and the bowling performance so far in the Game, on a Frame-by-Frame basis.
-	The User should be able to select the ball used for a Shot - and the System should remember which ball was last used so that the User does not have to enter the ball for every Shot.
-	The User can also specify different bowling balls for 1st and 2nd Shots, and for different lanes, and the System will automatically track and display that information, as well.

## Statistics

The bowler will be able to retrieve a wide array of statistics from the Games that they have bowled.  Those statistics (or "metrix" - it is called *RevMetrix* after all) will be represented in both **numeric** and **graphical** form:

-	**League Average**: the average of all Games bowled in a league
-	**Game Average:** averages of 1st Games, 2nd Games, 3rd Ggames bowled in a league
-	**Average Trend:** graph of average over the entire league, all leagues, all first Games over a date range, running sum average for a certain # of Games for a given date range, etc...
-	**High and Low Games:** across all Events, across a certain league, across certain 1st, 2nd, 3rd Games within a league, etc...
-	**Histograms of Scores:** distribution of 180's, 190's, 200's, 210's, 220's, etc., for a given Event or date range
-	**Pocket Percentage:** percentage of 1st Shot attempts that hit the pocket, percentage of pocket hits that resulted in strikes, etc...
-	**Pocket Quality:** percentage of light pocket hits, high pocket hits, solid pocket hits, and the percentage of each that resulted in strikes, and the types of leaves when not strikes
-	**Strike Percentage:** percentage of first Shots that are strikes (across all events, a league, across a date range, for a given ball, etc.)...
-	**Spare Percentage:** similar to the above for spare attempts
-	**Leave Percentage:** the percentage of leaves that are 10-pins, all single-pin leaves, splits, etc...
-	**Conversion Percentage:** the percentage of leaves that were converted (example: % of 10-pins made)
-	**Recent Performance:** a wide variety of other *metrix* for performance on strikes, spares, average, etc...
-	**AND SO MUCH MORE...**

<div class="callout">
**NOTE: These requirements are subject to change, at the whim of you pesky clients...  :-) **
</div>
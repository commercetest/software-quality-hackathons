# Software Quality Hackathons
A guide to help design and run hackathons where some improvements take a while to measure. To help everyone interested in this topic we will sometimes use a specific project - PocketCode - as an example.

## Context of the hackathons
We would like to use these hackathons to be a catalyst for helping contributors improve various aspects of the software quality of - typically - a specific project (e.g. PocketCode).

The software is likely to already exist and have active users. There will be at least one source of analytics that records and reports aspects of the software such as installs, active sessions, etc. The source(s) provide data to the project team which may augment and complement other sources of information such as test results, static analysis, code metrics, etc.

## Objectives
Ideally the hackathon will include some immediate measures of progress and improvements; in practice some of the measurements will be of a longer term nature, such as improvements in the crash rate once a new version of the software has been released and is being used in the field.

## Tips of what worked well at other hackathons
- Combining mixed teams
- having several iterations during the overall hackathon
- having something to create 
- Motivation for participants
- Pairing with a developer of the app to investigate possible causes of errors and other concerns.

## Less well
Creathon - didn't have anything material to create, more a think great thoughts, and wander around.

# Examples
## Catrobat Hackathon, Graz, Nov 2019
A relatively small group of under 10 people spent a day investigating the most frequent crashes and ANRs reported by Android Vitals for the Pocket Code Android app.
- After introductions and agreeing the aims of the hackathon we created individual tickets in the project's JIRA board for the top crashes and ANRs. We used a consistent tag in JIRA for each issue to make the group easier to track and report on.
- We worked in ones and twos (a developer of the app was in each group) on individual bugs.
- We tried to understand the possible trigger of the error, what were circumstances that would lead to the error occuring. We generally created a test to try to reproduce the error. And, where practical, we reproduced the error.
- We updated the JIRA tickets with our progress and findings.
- Where developers believed they knew enough to potentially ameliorate or fix the behaviour they revised the source code for the app and followed the project's usual review, code quality and testing practices. Their pull request was merged once it was believed to be better than the existing code.
- Owing to the relatively long release cycle and release process a new version of the app was released after the hackathon was completed. 
- The effects of the changes were tracked using a mix of user ratings and reviews in Google Play Console, Android Vitals, and Fabric Crashlytics console - all these were already in use by the project.

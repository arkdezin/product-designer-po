# Product Requirement Document (PRD)

## Background & Vision

We are building this learning module to provide better guidance to the RA's to fulfill their job properly so that the quality of the data collected is good and meets the client's requirement and standards for acceptance. 
The vision was to provide a robust and centralized place for the RA's to do the work, take the training, and be aware of what they need to do and what is the accepted quality of the data that they need to collect. 

## User Personas

So basically there are three personas that are directly or indirectly involved with this particular module. Starting with the first one, Research Associate

1. Research Associate - The person who needs to take the training 
2. the management team, including the field ops team - The person or the team which is responsible for creating trainings 
3. the client - The end user who is entitled to get quality data 

## MVP In-Scope vs. Out-of-Scope 

The scope was readjusted and slashed down a lot to match the requirements of the version 1 MVP due to time constraints and complexity in the building of those things. 

### In-Scope

on the web training module. on the mobile, taking that training and completing
on the web with the training capability of creating learning paths also.

- support video materials
- multi-choice type materials
- viewing of all the trainings
- assigning of trainings
- deleting of trainings
- adding the videos
- Ability to edit trainings, 
- delete uploaded videos

### Out-of-scope

- Complex Assignment Logic, 
- Dashboard to view Training Details,
- Restricting of Jobs based on Trainings Assigned 

## Functional Requirements

- The field ops training manager should be able to see the list of all training, including the draft training, active training, and archive training. 
- At the Field Ops Manager should be able to:
- Delete trainings
- Publish trainings
- Assign a RA to that training
- Duplicate a training or copy a training

There should be a training builder that lets them add:

- the training name
- training description
- learning path
- learning path order if the training belongs to a learning path
  The training builder itself should be able to add:
- video material
- multi-choice materials,
- The multi-choice materials should have the following capabilities:
  - They should have a field to add the question or the description.
  - They should have an option to add a reference image.
  - They should have an option to select the correct answer.
  - They should have an option to add the answer to the question.
  - They should have an option to choose if that particular multi-choice is a single-choice or a multiple-choice.

There should also be a capability to add videos separately in a video library and those videos will be utilized in the video material while creating the training. Also on that video library, the video training should have the following information:

- The video title
- When was it uploaded
- Who uploaded that video
- Certain actions like deleting that video or editing the title of that video

For the MVP V1 the assignment rule is very simple. The field ops training manager can either select the RA's from the list that is already available off the list of RA's or they can upload an Excel file with the email ID of those RA's to be selected from that list if they want to bulk select. Very simple.
This goes for both individual training and learning path. Once a person is assigned to a learning path, all the trainings within that learning path are available to that particular RA since that learning path is the one that is getting assigned not individual trainings. If the training is an individual training, that is only available to the RA who is assigned to that 

## Non-Functional Requirements

- Video streaming latency thresholds 
- accessibility (WCAG 2.1 AA) 
- concurrent user concurrency load 

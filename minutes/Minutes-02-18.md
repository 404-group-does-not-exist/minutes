# Minutes for Meeting 2 - Feb 18

## Agenda

1. Finalize Project Idea
   - discuss pros/cons
   - decide on project
3. Work on Milestone 1 questions
   - decide on implementation details
     - stack
     - host
   - review project management toolset


## What Was Discussed

We discussed 2 of our better ideas and sketched out 
what they might look like so we could weigh pros/cons.

**GOAL:  decide on our which idea to implement by recitation on wednesday**
so we can submit Milestone 1 this weekend. **Please** don't let this list 
stifle your creativity. If anyone gets inspired with a great idea before
the weekend let the group know. We're not really committed to anything until
we submit Milestone 1 and even then we're really not committed until we start
working on it.

### Idea 1: Radio Traffic: (wifi or ADSB)

This Idea initially started with the concept of using a Raspberry 
Pi or similar device to measure network traffic in a certain area 
of campus  (e.g. CSEL, the Library). By analyzing the amount of network
traffic with the device and then uploading the data to our web server,
our webapp could then tell a user whether or not the room was crowded.

There are two potential downfalls to this idea:
1. We may not be allowed to run our device on the university wifi (i.e. against policy or possibly illegal)
2. There is a large amount of network traffic data, the challenge would be to sift the data to get
   a reasonable estimate for the amount of people (i.e. phones) are trying to connect. 
   
#### Idea 1-A: Airplane Traffic

Instead of counting people, we would be looking at flight traffic overhead
This only requires an ADSB reciever and a pc to read the data. 
Potential expansions to this project are to overlay the flights on google maps
-can we query individual flight numbers?

### Idea 2: Event Message Board

This concept is sort of a craigslist/eventbrite clone but simpler and limited to CU.
The *Minimum Viable Product* here is a user can post an event that all others can see
Additional features could include:
- users can click a button to join/attend event
- users can click a button to ignore/hide an event on the list
- could implement primitive messaging between users

----
Here are the questions we need to answer for Milestone 1...Many have been answered,
at least partially.

## Milestone 1 Questions

*All of this will need to by typed up in a pdf for submission*

1. Team Number
   
   104-2
      
3. Team Name

   404 Group Not Found
   
5. Team Members

   Peng Jiang, Ryan Campbell, Jason Nguyen, Baiyu Chen, Jasper Niemeyer, Robert Cope

7. Application Name
8. Application Description
9. Vision Statement
10. Version Control

   Github
   
12. Development Method

    Agile Lite: The team will adopt some methods from the agile methodology, but not all. (*expound on this a little in the official milestone doc*)
    
14. Communication Plan

    Predomenantly GroupMe for discussion and Trello for TODO's
    
16. Proposed Architecture Plan

18. Meeting Plan

    Generally, Mondays from 5pm-7pm. Some team members can only be present for first half and others for second half. 
    

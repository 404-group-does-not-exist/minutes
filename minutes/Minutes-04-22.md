# Minutes for meeting on 04-22

- presentation coming May 1

- currently functioning login and data displaying at: [Roberts domain](https://wifiology.copesystems.com)

## Agenda

- discuss what exists  
- discuss final sprint
- discuss presentation

## what exists:

### wifiology running on copesystems

- not on heroku: why? 
  - hobby-dev db tier too limited,
  - PaaS hides too much

- deployed to a VM instead
  - advantage, hook up more monitoring tools

- login/registration working

- data is displayed and nicely

### ryan's android app

- login works

- test call to user main gets all users nodes

- gets last 20 measurements of each node

- checks for new SSID's

- tracks time

## Finalizing The App

### Distill data down to simple metric busy/not busy

### What goes in CSV export:
- unique mac addresses
- what network
- or leave as api call.
- both? use a dummy simple CSV plus op expose api key for custom export

### Andoid app --> similar to website

### website: 
- land on page and login/register--> marketing version of 1st paragraph last milestone
- busy/not colorcoded metric added to node view
  - use running average of traffic
  - yellow, near average
  - red, above average
  - green , below average

- glue in notifications
- testing in sellenium

## Presentation Stuff

- get slide show started -jasper
- assign people to be product manager/product owner -departments,scrum master,etc.

- pre-record product demos


## keep pushing, almost there!


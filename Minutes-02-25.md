# Minutes for Meeting 3 - Feb 25

## Proposed Agenda

1. Finalize app name and create repo
2. discuss how to contribute to repo
3. set up trello / discuss Kanban task management
4. discuss project architecture and initial goals
5. assign tasks for this week

## Finalize app name

its unanimous -> Wifiology is the name

repo created: https://github.com/404-group-does-not-exist/Wifiology

## Discuss Architecture

### On RasPi

Raspi plugs into radio
- has collection job: constantly running -> parse incoming data
- throw out unneeded data, cache needed data
- Run Cron Job periodically - Batch upload to DB
- collection job and cron job can be done in python or c++

Web Front End gets data from DB
- HTML, CSS, JS, NodeJS
- NodeJS takes place of PHP in traditional LAMP stack
  - i.e. Node handles read from DB

What goes in DB?
--schema design will inform other aspects of project

### Git hub stuff

Discussion of branching policy: <add links>



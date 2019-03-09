# Minutes for meeting 4 - March 4

## Proposed Agenda

- Features of App (**Need 6 total**)
- Milestone 2
   - Due Sunday March 10 @ 11:59pm
   - Product Feature List (title and description)
   - Requirements (functional and non-functional for at least 6 features)
   - Project Plan using Kanban
      - sequence of sprints - WHO, WHEN for feature implementation

## Proposed Functionality

Loosely prioritized

1. check traffic on node:
  - FUNCTIONAL REQ: allow users to check 802.11 traffic on a given node
   
  - NONFUNCTIONAL REQ: 80211 traffic can be used to provide an estimate for amount of people in the area of the node. Need to come up with a formula for that estimate.
   
2. list out available wifi connections
   - FUNCTIONAL: All the wifi base stations broadcast access points. App collects all available access points
   - NONFUNCTIONAL: no nonfunctional requirements here. List of access points should be accurate

3. list out traffic on each connection
   - FUNCTIONAL: Store a count of number of devices trying to access each access point, and report.
   - NONFUNCTIONAL: This is at its most accurate when a batch update has just finished on our DB. So to provide the best service minimize time between batch uploads without overwhelming the DB.
     
4. export data to CSV (for user use and for admin use)
   - FUNCTIONAL: Run report on DB -> transform to needed data output -> output data as CSV
   - NONFUNCTIONAL: Can be used for administrative tasks or to build future features which allow users to see perfomance metrics over time.

5. view time stamp of last batch update to DB
   - FUNCTIONAL: Time series data will contain timestamps
   - NONFUNCTIONAL: App may want to run another batch job if the timestamp is old.

6. Notifications (this can be a whole class of features)
   - FUNCTIONAL: user can recieve notification (email or phone) if node traffic above or below certain threshold
   - NONFUNCTIONAL: This email is sent immediately when node crosses threshold. 
     
     
8. Allow users to comment on node
9. Perfomance testing
10. Graph perfomance over time


### User profile

- name
- password
- email
- phone

### Robert's Proof of Concept notes

note: 2 DB's
1. cache (could be json)
2. Actual DB- postgres

#### Regimes

1. channel hopping (listen for beacon every 30sec or so)
2. for fixed amt of time capture everything
3. connect to AP and run standard TCP/IP or HTTP performance test

#### challenges

- 802.11 parsing
- schema for storing data from runs in cache

### Our Milestones (i.e. sprints)

- Sprint 1 - Implement Enablers
    - bare client -> log std out
    - db schema proposal
    - wire frames
    - basic front end
    - Node APP structure
    - research
      - User Auth/Hashing      - Ryan 
      - Hosting                - Jasper
      - Notifications          - Peng
      - 802.11 parsing (juicy) - Robert

- Sprint 2: Basic Query Implementation 
    - basic query implementation in app
      - first focus: user table, node table -> hashing library for auth
    - get client to updload basic data in batch jobs
    - investigate nofification services + research
    - login/logout (OAUth ? jwt? basic?)
     
- Sprint 3 API Implementation
   - start implementing features
   - more templated pages generated from DB dat
   - Finalize DB schema
   - Hook up notifications
   - Implement Auth

### Retrospective


- Plus: WE HAVE A PLAN!! good job Robert proof of concept, Jasper taking notes and leading meeting, Thanks for attending everyone. Thanks Jason for letting us book room. 
 
- Nuetral: s180C not the ideal room, 802.11 parsing will be hard but we did it to ourselves, 

- Negative: Difference between plans for milestones and the plan we need to implement is somewhat frustrating. 6 features is kind of arbitrary: it incentivizes trivial features over deep features(breaking with UNIX philosophy)


### Action Items

- pick cards on Trello
- ask questions when you get stuck


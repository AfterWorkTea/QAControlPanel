# QA Control Panel

QA Control Panel is an IT system meant to help QA professionals.

##Functionality
* collect and store test results 
* provide user-friendly panels to help evaluate results of the tests
* provide diagrams to show history/trends
* calculate and report Q/A metrics

##Software stack
* PHP
* MySQL
* Apache 
* HTML 5 + JavaScrtip

##Data structure
* Supports one or a few Projects (limited by server resources)
* Each Project groups one or a few Job
* Each Job can run multiple multiple times giving Builds
* A Build can run one or more tests
* Each Test can include one or more scenarios
* Running a Test with Scenarios generates result for each Scenario
* Each Test belongs to a Catalog of tests
* Each Catalog belongs to one and to only one Team
* All possible results are per-defined in an internal dictionary
* All current and historical Teams are per-defined in an internal dictionary

Project is described by a short, unique name name 
Job is described by a short, unique name name 
Build is described by a unique natural number kept in sequence
Test is described by a unique name
Scenario is described by a unique name
Catalog is described by a short, unique name name 
Team is described by by short, unique name name 

##GUI Panels and functions
* Project selection
* Recent Job/Build imports for the selected Panel
* List of imported Builds per specific Job
* Evaluation Pan showing individual Scenarios with reference to Tests/Catalogs/Teams with results that allows to manual assigned a new status with a comment, is shows build summary (arrogated results grouped by status, run time, build name)
* Diagram of passed/failed Tests/Scenarios per Build for a selected Job
* Diagram of number of Tests/Scenarios per Build for a selected Job
* Diagram of number run Builds per Job over day/week/month
* Report Test stability per Job
* Report top failing Tests/Steps per Job
* Report most common reasons (technical messages) for failing Tests  per Job

##Processes
* Import process for results of tests
* Email notification
* Chat notifications

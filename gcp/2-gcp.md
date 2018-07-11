# GCP Fundamentals

## Core Infrastructure

Projects are the main way you organize resources you use in GCP. Use them to group together related resources, usually because they have common business objectives.

There are 4 ways to interact with GCP management layers:
* Cloud Platform Console - Web user interface
* Cloud Shell and Cloud SDK - Command-line interface
* Cloud Console Mobile App - For IOS and Android
* REST-based API - For custom applications

### Resource hierarchy level
* Group your resources according to your organization structure
* Levels of hierarchy provide trust boundaries and resource isolation
![Alt text](images/Screen%20Shot%202018-07-10%20at%2010.46.38%20PM.png?raw=true "GCP hierarchy")

### Folders offer flexible management
* Folders group project under an organization
* Folders can contain projects, other folders, or both
* Use folders to assign policies

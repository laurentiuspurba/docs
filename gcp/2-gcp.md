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

## Identity Access Management IAM
Consits of:
* Who - can be defined by google account, google group, service account, entire G-Suite or cloud identity domain
* Can do what - IAM role (collection of permissions) 
* On which resources - 

### Type of roles of IAM
* Primitive - apply across all GCP services in project:
  * Owner - Invite & remove members, delete project and below
  * Editor - Deploy application, Modify code, configure service, and below
  * Viewer - Read-only access 
  * Billing administrator - Manage billing, add and remove administrators
* Predefined - Define where the roles can be applied; for example, Compute Engine offers a set predefined roles; Cloud Big tables offers role that can be applied across the entier organization to particular project or to individual big table instance
* Custom - 

## IAM Roles

## RESTful API
* Programatic access to products and services
  * Typically use JSON as an interchange format
  * User OAuth 2.0 for authentication and authorization
* Enabled through Google Cloud Platform Console

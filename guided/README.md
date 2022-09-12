# OrangIT Standard Documentation

Project purpose: What is the reason why this application exists? What real-world business cases does it support?

## Getting started

Prequisites: 
- What other software you need to have installed on your local machine in order to set up a development environment?
- Is there are separate file for environmental variables? 
- How does a developer get one that works?
- Are other changes - such as /etc/hosts, port-forwardings - needed?

Setup:
- Install dependencies and other initial setup steps e.g. `docker-compose up` and `npm install`.
- How to start the application locally e.g. `npm start`.

Access the application locally:
- What URL(s) to use to access the locally running application?
- What kind of credentials do you need to access all relevant pieces of the application?
- If there are multiple distinct user roles, you need a test user account for each of them.

## Architecture

High-level architecture: 
- what is deployed and where, what are the main integration points? 
- What are the main languages/technologies used? 
- What kind of data is stored and where?
    - Don't hesitate to use a picture.

## Development

### Run tests

- How to run tests locally? 
- Are there unit tests?
- Are there integration tests?
- Are there e2e tests?

Describe here how to run any/all of them.

### Migrations

How to run database migrations locally (if necessary). Sometimes the migrations are run as part of the test suite, which is preferable.

### How to make a production data dump and import it into the local development environment?

Sometimes you run into hard-to-reproduce bugs, which manifest themselves only with production data.

In those cases it is extremely useful to be able to do a data dump from production and set up the local
development environment with production data.

Describe how to do that here.

### Repository guidelines

If using git:
- What kind of git workflow is used in this project. Merge or rebase?
- Should commits be squashed, and if yes, in which circumstances?
- What are the requirements for commit messages?
- What are the naming conventions for branches?
- All other git-related stuff that comes to mind.

If using some other version control than git:
- The same as above, as is relevant to the version control system in use.

Code style:
- Coding conventions, linting, etc.

## Test environment

### Access

- The URL where the test environment of the application can be found.
Also, all other URLs which point to something relevant, like for example an administrator UI, etc.
- The credentials to use in the test environment. For example, username and password. If there are multiple
distinct user roles with different access to some parts of the application, there must be multiple developer accounts
in order to be able to test all of them.
- If a VPN, SSH tunneling or some other similar way to access the test environment is required,
describe the steps needed here.

### Deployment

- How a deployment is done.
- The steps needed to verify that a new version is running in the test environment successfully.
- Tests (scripts or otherwise) that you have to run in order to ensure that a deployment was successful.
- Things that you have to test manually in order to ensure that a deployment was successful.
- How to restore the previous version of the software when a deployment goes wrong?

### Logs

Where are the logs, how to change logging levels, etc.

### Monitoring

What kind of monitoring is there in the test environment, if any.

## Production environment

### Access

- The URL where the production environment of the application can be found.
Also, all other URLs which point to something relevant, like for example an administrator UI, etc.
- The credentials to use in the production environment. For example, username and password. If there are multiple
distinct user roles with different access to some parts of the application, there must be multiple developer accounts
in order to be able to test all of them.
- If a VPN, SSH tunneling or some other similar way to access the production environment is required,
describe the steps needed here.

### Deployment

How a production deployment is done.

### Verifying that a deployment was successful

The steps needed to verify that a new version is running in production successfully.

#### Automated test cases

Tests (scripts or otherwise) that you have to run in order to ensure that a deployment was successful.

#### Manual test cases

Things that you have to test manually in order to ensure that a deployment was successful.

### Rollback

How to restore the previous version of the software when a deployment goes wrong?

### Logs

Where are the logs, how to change logging levels, etc.

### Monitoring

What things are monitored? Which tools are used? How to access the UI(s) of the monitoring tools?

## Continuous integration

Where is/are the CI(s) for this project?

## Operating instructions for manual and semi-manual processes

Many applications require some manual processes which occur from time to time, like for example
adding new users, doing manual database maintenance work, creating monthly reports etc.

Describe how to do them here. The descriptions have to be detailed enough so that someone else can do them
with these instructions.

## More useful information, Tips and Tricks

- Other important or useful things to know.
- Security considerations: Are there any specific things to consider regarding the security of the project, in addition to the usual best practices?

IDE setup:
- If there are some special tricks needed to get the project working in IDEA/Eclipse/something other, then
describe them here. Preferably attach screenshots, if applicable.


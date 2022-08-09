## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

---

## Write a Git Guide


## Why another course?

We have two ways of writing the guides
1. Through the UI
2. Through Git

Git options provides a couple of benefits
1. Review's can be done via PRs
2. People across the project can for the repository and contribute
3. Content is backed-up
4. Content is Open Source and can be used by everyone


    


---
## Evaluation





##### Why do we write git based guides instead of using the UI option?  

- [x]  People across the project can for the repository and contribute
- [x]  Review's can be done via PRs
- [ ]  Git based guides have more features as compared to UI based guides
- [x]  Content is Open Source and can be used by everyone

    


---
## Guide Files

When adding a new guide you will have to add a new YAML file in `src` directory.

We then need to add the entry of that file in `guides.yaml` file. 

e.g. see this repository [https://github.com/DoDAO-io/dodao-aave-guides](https://github.com/DoDAO-io/dodao-aave-guides)

We add guide files in yaml format. The reason we use YAML format is because it is easier to write a YAML as compared to JSON. Also, YAML provides easy way to work with multi-line strings.

With-in the course YAML files, we have content field for step and stepItems. This field can contain multi-line strings. The contents of these multi-line strings can be in Markdown format.

If you are willing to contribute, it is very important that you understand the basics of YAML and Markdown format

## Learn YAML
You can go through these tutorials or watch any of the youtube videos on YAML

[https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)

[https://www.tutorialspoint.com/yaml/index.htm](https://www.tutorialspoint.com/yaml/index.htm)

## Learn Markdown
You can go through these articles or watch any of the youtube videos on Markdown

[https://www.markdowntutorial.com/](https://www.markdowntutorial.com/)

## Setup
Use a proper IDE that can validate yaml file and also that shows markdown in view format.


    


---
## Evaluation





##### What markup language/s do we use for writing course files?  

- [ ]  We just use YAML format
- [x]  File is on YAML format and the some of the fields can be represented as multi-line Markdown string
- [ ]  Files are in JSON format
- [ ]  File is in Markdown format and the some of the fields can be represented as multi-line YAML string





##### What is the main reason to use YAML files for course files?  

- [ ]  YAML files are auto validated
- [ ]  YAML is easy to use in JavaScript
- [ ]  YAML is easier to learn than JSON
- [x]  It is easier to represent multi-line strings in YAML format

    


---
## Guide contents

A Guide consists of following things
1) Basic Info - This includes name, excerpt, thumbnail,  etc.
2) Steps - Here is the example of the step
   ```yaml
     - uuid: bd8f0b48-4e61-478a-b275-68e3c93db760
       content: |
       Currently contributing to courses involves working on a chapter which
       has \"two\" tasks
         1. Readings and Summaries - Create yaml file with details of readings and summaries for that chapter. e.g. [https://github.com/DoDAO-io/dodao-solidity-course/blob/main/src/summaries/data_types.yaml](https://github.com/DoDAO-io/dodao-solidity-course/blob/main/src/summaries/data_types.yaml)
         2. Questions - Create 50 high quality single or multiple choice questions for the  chapter you are working on. e.g. [https://github.com/DoDAO-io/dodao-solidity-course/blob/main/src/questions/data_types.yaml](https://github.com/DoDAO-io/dodao-solidity-course/blob/main/src/questions/data_types.yaml). Later
            on we will add another task i.e. creating of the mind maps for each chapter, but
            for now its not needed. Also make sure that your name is added on a Trello card corresponding to the task you are working on.
            stepItems: []
            name: Contributing
   ```
   Steps consist of following information
   1) UUID - unique identifier. You can use this site to generate a V4 uuid https://www.uuidgenerator.net/version4
   2) Name
   3) Content - Details that are rendered below the headings. This is a string formatted with markdown
   4) StepItems - Step items can be of the following types
      1) Question - Type of question can be `MultipleChoice` or `SingleChoice`
            ```yaml
               - uuid: f12c2758-858d-4fe4-9560-f4dd9454f89a
                 content: What two tasks are currently part of the work involved for a chapter
                 of a course?
                 type: MultipleChoice
                 answerKeys:
                 - B
                 - C
                 choices:
                 - content: Create a youtube video
                   key: A
                 - content: Create yaml file with readings and summaries
                   key: B
                 - content: Create yaml file for questions
                   key: C
                 - content: Create a mind map
                   key: D
            ```
      2) UserInput - This is used to capture information from user. Type can be `PublicShortInput` or `PrivateShortInput` e.g.
            ```yaml
                    - uuid: 5e025ae8-daf2-4074-8e6c-68de05d3e5cc
                      label: Name
                      required: true
                      type: PublicShortInput
            ```
      3) Discord - This step item is used to ask user to connect their discord. e.g.
        ```yaml
           - uuid: 0d3bf837-e661-43b3-ba85-6d2ebb272be5
             type: UserDiscordConnect
        ```

## Creating/Updating a Guide
When creating or editing a guide, create a new branch and after you are done with editing the guide create a PR


    


---
## Evaluation





##### Which one of these is not present under a step  

- [ ]  content
- [x]  explanation
- [ ]  uuid
- [ ]  stepItems
- [ ]  name





##### Which one of these is not a type of step item  

- [ ]  Question
- [ ]  UserInput
- [ ]  Discord
- [x]  Telegram

    


---
## Your Info

Create an account on Trello as we use that for task management [https://trello.com](https://trello.com)



| Label | Type | Required |
| ----------- | ----------- | ---- |
| Name        | PublicShortInput   |  true    |






| Label | Type | Required |
| ----------- | ----------- | ---- |
| Trello Username        | PublicShortInput   |  true    |






| Label | Type | Required |
| ----------- | ----------- | ---- |
| Github Username        | PublicShortInput   |  true    |




    


---
## Footer
This is the git footer. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.
    

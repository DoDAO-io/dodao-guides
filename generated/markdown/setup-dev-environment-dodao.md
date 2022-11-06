## Header
This is the course header. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.

---

## Setup Dev Environment


## Introduction

### Type of Content
In DoDAO we primarily write three type of contents
1. Guides
2. Courses
3. Articles

### Contributing to guides and courses
The best way to contribute towards creating or updating guides or courses is by editing the files in git repositories and then creating a pull request for reviews. This way, we can review the content that you write and make sure it meets our standards.

### Pre-requisites
#### Learn YAML
You can go through these tutorials or watch any of the youtube videos on YAML

[https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started](https://www.cloudbees.com/blog/yaml-tutorial-everything-you-need-get-started)

[https://www.tutorialspoint.com/yaml/index.htm](https://www.tutorialspoint.com/yaml/index.htm)

#### Learn Markdown
You can go through these articles or watch any of the youtube videos on Markdown

[https://www.markdowntutorial.com/](https://www.markdowntutorial.com/)

#### Learn Git
You can go through this tutorial or watch any of the youtube videos on YAML

https://www.youtube.com/watch?v=tRZGeaHPoaw

    


---
## Evaluation





##### What are the prerequisites for contributing to the courses?  

- [ ]  Markdown and YAML
- [x]  YAMl, Markdown and Git
- [ ]  Git and Markdown
- [ ]  None of these





##### What are the primarily contents we write in DoDao?  

- [ ]  Only Courses
- [ ]  Articles and Guides
- [x]  Guides, Courses and Articles
- [ ]  Codes for DeFi

    


---
## Guide Repo Structure

Any of the guides repositories like [https://github.com/DoDAO-io/dodao-academy-guides](https://github.com/DoDAO-io/dodao-academy-guides) have the following structure.
```
|--- LICENSE
|--- README.md
|--- generated
|     |--- json
|     |     |--- guide-file-1.json
|     |     |--- guide-file-2.json
|     |     |--- guides.json
|     |--- markdown
|         |--- guide-file-1.md
|         |--- guide-file-1.md
|--- package.json
|--- src
|     |--- guide-file-1.yaml
|     |--- guide-file-2.yaml
|     |--- guides-footer.md
|     |--- guides-header.md
|     |--- guides.yaml
|--- yarn.lock

```
Important things to keep in mind are 
1. All the content to be added or updated needs to be written in `yaml` files i.e. under `src` directory
2. All the files under `generated` directory are the files generated from the yaml files after we run `yarn test`
3. Files under `generated/json` are used by the app to render guides in the browser
4. Files under `generated/markdown` can be used by you to check the formatting of the content
5. Before you create a pull request, make sure to run `yarn test` and also checkin the generated files.

Note: If you add a new file, make sure to include it in the `src/guides.yaml`.

    


---
## Evaluation





##### Courses and Guides are written in which format?  

- [ ]  Markdown format
- [ ]  HTML format
- [ ]  Json format
- [x]  YAML Format





##### What must be done before creating a pull request?  

- [ ]  Run `node guides.js `
- [ ]  Include MIT license in the license directory
- [x]  Run `yarn test` successfully and do a check in generated markdown files
- [ ]  Run `yaml test` and correct the errors





##### Which directory's files need to be modified for guides?  

- [x]  src
- [ ]  generated
- [ ]  generated/json
- [ ]  package.json

    


---
## Course Repo Structure

```
.
|--- LICENSE
|--- README.md
|--- generated
|   |--- course.json
|   |--- explanations
|   |      |--- aave-smart-contracts.md
|   |--- questions
|   |      |--- aave-smart-contracts.md
|   |--- readings
|   |      |--- aave-smart-contracts.md
|   |--- summaries
|   |      |--- aave-smart-contracts.md
|   |--- topics
|          |--- aave-smart-contracts.md
|--- images
|   |--- aave.jpg
|   |--- architechture.png
|--- package-lock.json
|--- package.json
|--- src
|   |--- course-header.md
|   |--- course.yaml
|   |--- explanations
|   |      |--- aave-smart-contracts.yaml
|   |--- questions
|   |      |--- aave-smart-contracts.yaml
|   |--- readings
|   |      |--- aave-smart-contracts.yaml
|   |--- summaries
|          |--- aave-smart-contracts.yaml
|--- yarn.lock
```

Important things to keep in mind are 
1. All the content to be added or updated needs to be written in `yaml` files i.e. under `src` directory
2. All the files under `generated` directory are the files generated from the yaml files after we run `yarn test`
3. `generated/course.json` is used by the app to render the course in the browser
4. Files under `generated` folder can be used by you to check the formatting of the content
5. Before you create a pull request, make sure to run `yarn test` and also checkin the generated files.

Note: If you add a new file, make sure to include it in the `src/course.yaml` file under the right topic.


    


---
## Evaluation





##### The summary should be added to which directory?  

- [ ]  src/explanations
- [x]  src/summaries
- [ ]  src/questions
- [ ]  src/readings





##### What are some important things that should be taken care of after editing the files?  

- [x]  Make sure to update the different uuid's for the added files
- [ ]  Use different subtopics for all the 4 files
- [x]  Make sure the file name is same in all the four folders(explanations,summaries,questions, readings)
- [ ]  Change the compiler version in the package.json file





##### Where you can find the generated markdown files?  

- [ ]  It will be in package.json
- [ ]  It will be in course.json
- [x]  It will be in the generated directory
- [ ]  It can be viewed in Dodao.io

    


---
## Setup Your Editor

To edit the Yaml files use a code editor. We recommend https://code.visualstudio.com

Install the following plugins in your code editor
1. **Git** - This plugin can make it easy for you to see which files you have modified and allows you to checkin the code from the code editor itself.
2. **Yaml** - Yaml files follow a particular format and the plugin highlights the code in different colours making it very easy for you to add or update the content.
3. **Markdown** - We process the yaml files and then generate the metadata in markdown format. By installing markdown viewer, you can check the formatting of the markdown files. For guides and courses both, we generate markdown files, which you can open in the markdown viewer and check the formatting



    


---
## Evaluation





##### What is the preferred editor for editing YAML files?  

- [ ]  Sublime text
- [x]  Visual studio code
- [ ]  Notepad++
- [ ]  Dev c++





##### Which essential plugins and packages need to be installed?  

- [ ]  Github desktop and python plugins should be installed
- [ ]  Only git and YAML is enough. Npm package manager should be installed
- [x]  Git, YAML and markdown plugins. Yarn package should be installed
- [ ]  Node js must be installed





##### What plugin may be used to highlight keywords in yaml files?  

- [ ]  coderunner plugin
- [ ]  git extension
- [x]  YAML extension
- [ ]  markdown extension

    


---
## Creating Pull Requests

<div style="position: relative; padding-bottom: 56.25%; height: 0;"><iframe src="https://www.loom.com/embed/2de7bae66bd94d36834df18e8e85cc90" frameborder="0" webkitallowfullscreen mozallowfullscreen allowfullscreen style="position: absolute; top: 0; left: 0; width: 100%; height: 100%;"></iframe></div>
<br/>
<br/>
<br/>
<br/>
<br/>
<br/>

Few things to keep in mind
1. Setup ssh keys in github as explained here https://docs.github.com/en/authentication/connecting-to-github-with-ssh/adding-a-new-ssh-key-to-your-github-account.  This will allow you to commit and push your commits
2. Make sure you have access to the main repository to be able to create a new branch and commit to it. If you don't have access, contact a team member.
3. Make sure you run `yarn test` and also commit the generated files
4. After you create a pull request in github, make sure there are no merge conflicts

    


---
## Evaluation





##### What has to be configured for push and pull commits?  

- [x]  Set up ssh keys in github
- [ ]  Set up trello account
- [ ]  Setup hypertext terminal
- [ ]  Login the vscode with github account





##### Prior to making a pull request, what should be done?  

- [x]  Create a new branch and add the changes in the new branch
- [ ]  Make changes in the main branch
- [x]  Make sure that the pr has no merge conflicts
- [ ]  Add the ssh keys in the end of the yaml file





##### What should you do if you don't have access to create a new branch?  

- [ ]  Contact Ethereum community
- [ ]  Fork the repository and create a new branch
- [ ]  Get authorisation from github by mail
- [x]  Contact a team member

    


---
## Your Info





| Label | Type | Required |
| ----------- | ----------- | ---- |
| Your Name        | PublicShortInput   |  true    |




    


---
## Footer
This is the git footer. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.
    

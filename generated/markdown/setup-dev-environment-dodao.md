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
#### Setup
Use a proper IDE that can validate yaml file and also that shows markdown in view format.  

    


---
## Guide Repo Structure

Any of the guides repositories like [https://github.com/DoDAO-io/dodao-academy-guides](https://github.com/DoDAO-io/dodao-academy-guides) have the following structure.
```
|--- LICENSE
|--- README.md
|--- aa.txt
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


    


---
## Course Repo Structure

```
.
|--- LICENSE
|--- README.md
|--- aa.txt
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


    


---
## Setup Your Editor

To edit the Yaml files use a code editor. We recommend https://code.visualstudio.com

Install the following plugins in your code editor
1. **Git** - This plugin can make it easy for you to see which files you have modified and allows you to checkin the code from the code editor itself.
2. **Yaml** - Yaml files follow a particular format and the plugin highlights the code in different colours making it very easy for you to add or update the content.
3. **Markdown** - We process the yaml files and then generate the metadata in markdown format. By installing markdown viewer, you can check the formatting of the markdown files. For guides and courses both, we generate markdown files, which you can open in the markdown viewer and check the formatting



    


---
## Creating Pull Requests



    


---
## Footer
This is the git footer. This will be added on top of every page. Go to [DoDAO.io](https://www.dodao.io) to know more.
    

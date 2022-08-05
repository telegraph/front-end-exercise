# Front-End Coding Test

:wave: Welcome to The Telegraph front-end candidate test

- [Task](#wrench-task)
	- [Requirements](#mega-requirements)
	- [What we are looking for](#mag_right-what-we-are-looking-for)
	- [Data](#open_file_folder-data)
	- [Designs](#art-designs)
- [Set up](#floppy_disk-set-up)
- [Acceptance criteria](#scroll-acceptance-criteria)
- [Submitting your code](#mailbox_with_mail-submitting-your-code)

## :wrench: Task

We would like you to build a responsive commenting component as per the included designs. You should meet the [ACs](#scroll-acceptance-criteria).

Some basic front-end tooling ([webpack](https://webpack.js.org/) for JavaScript compilation and [PostCSS](https://postcss.org/) for CSS concatenation) has been provided.

You are not expected to complete the task, however you can write `// TODO`s throughout your code.

### :mega: Requirements

* Match the [designs](#art-designs) as closely as possible, filling in any gaps as you deem fit

### :mega: Requirements
* Application should be somewhat responsive (don't worry about this too much)
* Pass the [ACs](#scroll-acceptance-criteria)
* Comments should be called once the DOM is ready via [this endpoint](https://my-json-server.typicode.com/telegraph/frontend-exercise/comments). This call should be made client-side and injected with JavaScript.
* Keep your JavaScript vanilla please :icecream:

### :mag_right: What we are looking for

* An understanding of web fundamentals
* Ability to translate designs into code
* A consistent and scalable approach to the test
* An understanding of accessibility
* Reasoning about SEO

### :open_file_folder: Data

[https://my-json-server.typicode.com/telegraph/frontend-exercise/comments](https://my-json-server.typicode.com/telegraph/frontend-exercise/comments)

### :art: Designs

* There are exported design files in the `design` directory in the root of the project.

## :floppy_disk: Set up

Firstly, install all of the packages:

```sh
npm install
```

Then run the watcher:

```sh
npm run dev
```

Visit [http://localhost:3000/](http://localhost:3000/) in your web browser and you *should* see a blank webpage with The Telegraph logo and a 'Hello World' message.

The above command will watch and deploy your code. The watchers for CSS and JS files will not take into account changes to new files so make sure you restart the watchers when adding new files. The CSS watcher will only look for changes inside a directory which sits within the `src/css` directory (e.g. `src/css/elements`).

## :scroll: Acceptance criteria

```
Scenario: Show comments
	Given that I access the homepage
	Then the home page should return comments
	And each comment should show the username
	And each comment should show the comment body
	And each comment should show the like count
```

```
Scenario: Order comments by likes
	Given that I click the Likes button in the comments area
	Then then the comments should display in order of most likes
	And the comments should show most liked first
```

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

Your code should work in modern browsers such as Chrome, Firefox and Edge. Do not worry about supporting IE11 or below.

You should spend around one and a half hours on this task. If you do not complete the task in time please submit with a list of what you would have done with more time. Feel free to be specific and write `// TODO`s throughout your code.

### :mega: Requirements

* Match the [designs](#art-designs) as closely as possible, filling in any gaps as you deem fit
* Application should be fully responsive
* Pass the [ACs](#scroll-acceptance-criteria)
* Ensure code is unit tested. We've set this up with [Jest](https://jestjs.io/) but feel free to use whatever you like
* Comments should be called once the DOM is ready via [this endpoint](https://my-json-server.typicode.com/telegraph/frontend-exercise/comments). This call should be made client-side and injected with JavaScript.
* Keep your JavaScript vanilla please :icecream:

### :mag_right: What we are looking for

* An understanding of web fundamentals
* A consistent and scalable approach to the test
* An understanding of accessibility
* Reasoning about SEO
* Solid unit testing
* Ability to translate designs into code

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

## :mailbox_with_mail: Submitting your code

:no_entry_sign: Please don't fork this repository as the links will be accessible to other candidates. 

:heavy_check_mark: Please clone it into your own repo and send us a link. 

:heavy_check_mark: We should be able to build and run your application locally.

:heavy_check_mark: Please also feedback on how you found the test - what did you like/not like about it?

:heavy_check_mark: Feel free to send us any other additional notes. E.g. what you would have done with more time.

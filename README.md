# Professional-README-Generator with Node.js and ES6+

## Description 
  
The Professional README Generator is a command-line application that runs with Node.js and dynamically generates a README.md file based on user input about a project. Check out the [`ExampleREADME.md`](https://github.com/alexbachicha/Professional-README-Generator/blob/master/ExampleREADME.md) in this repo as an example. 


## Table of Contents
* [Installation](#installation)
* [Usage](#usage)
* [License](#license)
  

## Installation

*Steps required to install project:*

To generate your own README, first run `npm install` in order to install the following npm package dependencies:
  * [`inquirer`](https://www.npmjs.com/package/inquirer) that will prompt you for your inputs from the command line 
  * [`axios`](https://www.npmjs.com/package/axios) to fetch your info from the GitHub API

The application itself can be invoked with `node index.js`.


## Usage 

*Instructions and examples for use:*

![Gif demo of README-Generator](demo.gif)

When you run `node index.js`, the application uses the `inquirer` package to prompt you in the command line with a series of questions about your GitHub and about your project.

The application then takes your responses and uses `axios` to fetch your GitHub profile from the [GitHub API](https://developer.github.com/v3/), including your GitHub profile picture (avatar) and email.
From there, the application will generate markdown and a table of contents for the README based on your responses to the Inquirer prompts (if you don't answer the optional questions, such as Installation, an Installation section will not be included in your README). The README will also include badges for your GitHub repo.

Finally, `fs.writeFile` is used to generate your project's README.md file.


## License

MIT License

---

## Questions?

GitHub: [@alexbachicha](https://github.com/alexbachicha)

Email: agbachicha@outlook.com

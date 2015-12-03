# Personal Growth Assistant - Final mini-Project #1
---

Links:

- Instructions:
	- https://github.com/ga-students/wdi_lettuce_students/blob/master/schedule.md

- Project:
	- GitHub
		- https://github.com/madhat5/Personal-Assitant_appProject
	- Heroku
		- 
	- Trello link
		- https://trello.com/b/79qQIpKD/wdi-project-4a-jmny
	- Wireframes
		- 

---
Technical Requirements:

- Use Mongo & Express to build an API and a front-end that consumes it
- Create an API using at least 2 related models, one of which should be a user
- Include all major CRUD functions in a RESTful API for at least one of those models
- Consume your own API by making your front-end with HTML, Javascript, & jQuery
- Add authentication to your API to restrict access to appropriate users
- Layout and style your front-end with clean & well-formatted CSS
- Deploy your application online so it's publically accessible

---
Timeline goals:

- Wed 12/2 --x--
	- Start planning Rails app today (and others)
- Sat 12/5
	- Rails app finished during the weekend
- Sun 12/6 --o--
	- Start planning Mean App 
- Wed 12/9
	- Mean app finished 
- Thu 12/10
	- Final project planning
- Thu 12/17	
	- Final project finished

--
Deployment flow:

- Create development branch
	- from master
		- git checkout -b development		
- Pull @ beginning of day
	- from development
		- git pull origin master
		- (npm install) if needed
- Create 1 branch per file feature
	- from development
		- git checkout -b file_feature
- By end of day 
	- from branch
		- git add .
		- git commit -m "update details"
		- git push origin file_feature
		- (gitHub
			- Pull request)
		- OR
		- (git push origin development)
		- git checkout development
	- from development
		- (gitHub
			- Pull request)
		- OR
		- (git push origin master)

---
MVP

Models:

- user
	- stormpath
	- goal (embed or ref)
- goal

User story:

- MOAR MODALS!!!

- landing page:
	- map
		- modal for location details
		- cannot add location until logged in
	- log in button
		- > opens user page
	- register buton
		- > opens register form

- user page
	- map
		- modal dislpays
			- task
			- location
			- details
			- button add to to-do
	- to do list (div)
		- task
		- button complete
			- complete pushes to Done
	- user updates button
		displays form 
		- edit
		- 
	- logout

+features:

- 


---
---
App Build Steps:

- yo ...

- stormpath
- angular



- touch server.js --x--

- npm init --x--
    - 'enter' through all the prompts

- express setup (npm install --save express) --x--
    - server.js
    	- var express = require('express');
		- var app = express();

- set app port --x--
    - server.js
        - var port = process.env.PORT || 3000;

- morgan setup (npm install --save morgan) --x--
    - server.js
        - var morgan = require('morgan');
        - app.use(morgan('dev'));

- bodyparser setup (npm install --save body-parser) --x--
    - server.js
        - var bodyParser = require('body-parser');
        - app.use(bodyParser.urlencoded({ extended: false}));
        - app.use(bodyParser.json());

- mongoose setup (npm install --save mongoose) --ox--
    - server.js
        - var mongoose = require('mongoose');
        - mongoose.connect('mongodb://localhost/db_name');

- md5 setup (npm install --save md5) --x--
	- server.js
		- var md5 = require('md5');

- cookies setup (npm install --save cookie-parser) --x--
	- server.js
		- var cookieParser = require('cookie-parser');
		- app.use(cookieParser());

- mkdir public --x--
	- server.js
		- app.use(express.static('public'));
	- touch public/index.html
	- touch public/app.js
	- touch public/style.css

- middleware setup --x--

- models --ox--
	- mkdir models
		- touch models/user.js
		- touch models/task.js
	- server.js
		- var User = require('./models/user');
		- var Task = require('./models/task');

- test connection --o--
	- setup basic route
	- setup basic index.html/app.js
	- launch server (nodemon)

- CDN
	- Handlebars URL --x--
	- js-cookie URL --x--
		
- model build --o--
	- user.js
		- var mongoose = require('mongoose');
		- var userSchema = new mongoose.Schema({ ... });
			- link taskSchema
		- var User = mongoose.model('User', userSchema);
		- module.exports = User;
		- embed tasks (ref Complaints)
	- task.js
		- var mongoose = require('mongoose');
		- var taskSchema = new mongoose.Schema({ ... });
		- var Task = mongoose.model('Task', taskSchema);
		- module.exports = Task;
		- ?embed users?

- Story build --o--
	- server: 
		- server.js 
			- TEST 
	- client: --o--
		- TEST
		- index.html
		- app.js
			- user 
				- signup
				- update
				- delete
			- task
				- all
				- new
				- delete (auto delete when done)

- CSS --o--

- node server.js


---
---
Reference

- Git merging
	- https://github.com/ga-students/wdi_lettuce_students/blob/master/w08/d02/INSTRUCTOR/git_solo.md





---
---
Comments

- 



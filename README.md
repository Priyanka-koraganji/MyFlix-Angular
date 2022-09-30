# MyFlix-Angular
General notes on this Angular project
This project was generated with Angular CLI version 13.3.5.

Development server
Run ng serve for a dev server. Navigate to http://localhost:4200/. The application will automatically reload if you change any of the source files.

Code scaffolding
Run ng generate component component-name to generate a new component. You can also use ng generate directive|pipe|service|class|guard|interface|enum|module.

Build
Run ng build to build the project. The build artifacts will be stored in the dist/ directory.

Running unit tests
Run ng test to execute the unit tests via Karma.

Deploy to gh-pages
Run ng deploy --base-href=/MyFlix-Angular/

Further help
To get more help on the Angular CLI use ng help or go check out the Angular CLI Overview and Command Reference page.

Description
The aim of this project is to build the client-side for an application called myFlix using Angular based on its existing server-side code (REST API and database), with supporting documentation.

User Stories:
As a user, I want to be able to receive information on movies, directors, and genres so that I can learn more about movies I’ve watched or am interested in.
As a user, I want to be able to create a profile so I can save data about my favorite movies.

Key Features:
Welcome view where users are able to either log in or register an account
Upon authentication, display a view of all Movies
Upon clicking on a particular movie, users will be taken to a single movie view, where additional movie details will be displayed. The single movie view will contain the following additional features:
A button that when clicked takes a user to the ​director view,​ where details about the director of that particular movie will be displayed.
A button that when clicked takes a user to the ​genre view,​ where details about that particular genre of the movie will be displayed.
What technology did I use and why?
I chose to create the application using Angular due to the following considerations:

I use Angular Material to style the UI of my application to make it responsive and take advantage of the ready to use components, such as mat cards.

What challenges did I face, what did I learn?
The Profile page needs to display Favorite Movies of the user. Yet that needs to be done.

Development Process for the movies application:-
Install Angular
Check if Angular is already installed on device
ng --version
If not, install Angular
npm install -g @angular/cli
Create a new Angular project
Navigate to folder and create project
ng new my-project-name
Navigate to project folder to run project
ng serve --open
Set up app to load data from movie API
Set up Angular HttpClient 1.1. Go to app.module.ts and add
import { HttpClientModule } from '@angular/common/http';
Add HttpClientModule to the imports of @NgModule
Create Angular Service for Consuming REST API 
Create a new Service inside app folder
ng generate service fetch-api-data
Add modules to imports array to serve to other components
Create components for user to use application
$ ng generate component my-component-name
Create routes in app.module.ts
Deploy application on github pages
If not done yet: Create github repository for application
If also not done yet: Link the new remote repository to the local project folder. To do so, simply run this command from inside your project folder (replace and with your own GitHub username and repository name): git remote add origin https://github.com//.git
Add angular-cli-ghpages by running
--ng add angular-cli-ghpages.
Build your application (i.e., generate static HTML, CSS, and JavaScript files out of your application so that browsers can interpret them without the need to use any extra tools/plugins). To do so, run the following command, replacing with your own repository name:
--ng deploy --base-href=/<repository-name>/.
Add TypeDoc Documentation
Install typedoc (if not yet installed):
--npm install typedoc
Check that code is commented adhering to best practices
Run typedoc to create documentation

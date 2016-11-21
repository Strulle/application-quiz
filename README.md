# ApplicationQuiz

Objects: 
Question
  question_text  
  Time:number
  TakenTime:number
  

SingleChoice implements Question
  PossibleAnswers:array<Sring>
  GivenAnswer:String

MultipleChoice implements Question
  PossibleAnswers:<String>
  GivenAnswers:array<String>

FreeText implements Question
  GivenAnswer:string


Attendee
  firstname
  lastname
  email


Sample Routes:
/quiz/welcome/      //Get User Info
/quiz/question/:id  //guarded
/tranmission        //guarded
/thanksgiving       //guarded

Singelton Services:
  attendee.service
  questions.service
  progressbar.service
  timer.service
  inputvalidation.service
  routeguard.service
  transmission.service


possible functions Server-Side-Application
  Create Session for Attendee
  Compare sum of TakenTimes with time between request questions an submitting answers on ServerSide to prevent manipulation  

This project was generated with [angular-cli](https://github.com/angular/angular-cli) version 1.0.0-beta.19-3.

## Development server
Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive/pipe/service/class`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).
Before running the tests make sure you are serving the app via `ng serve`.

## Deploying to Github Pages

Run `ng github-pages:deploy` to deploy to Github Pages.

## Further help

To get more help on the `angular-cli` use `ng --help` or go check out the [Angular-CLI README](https://github.com/angular/angular-cli/blob/master/README.md).

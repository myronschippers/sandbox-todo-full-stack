# Process Notes

## Video 1, Initial Backend Application Setup

1. Install Dependencies, [nvm](https://github.com/nvm-sh/nvm), [git](https://git-scm.com/download/mac), and [nest cli](https://docs.nestjs.com/first-steps)
    - MacOS `brew install nvm`
    - MacOS `brew install git`
    - after node is installed run `npm i -g @nestjs/cli`
1. Initial setup
    - initialize Nest starter application
    - `nest new todo-app`
1. Run initial application (is it working)
    - ??? `npm install` ???
    - `npm run start`
    - application is running at [localhost:3000](http://localhost:3000/)
    - what is `ctrl` + `c` (stop the application from running)
1. Structure
    - make a GET route "say-something", in `/src/app.controller.ts` create `@Get('say-something')`
    - add a test to the `/src/app.controller.spec.ts`, `describe()`
    - run the test to see if it passes, `npm run test`
    - what is test coverage???, `npm run test:cov`
      - run everything with `npm run test && npm run test:cov`
    - returning a simple string
    - `npm run start` vs `nvm run start:dev`
    - move string for `/say-something` route to the `/src/app.service.ts`
      - using a new string value for the message, "New Message"
      - refresh route in browser and see new message but app is running but what about the test
    - check the tests `npm run test`
1. Adding to a GitHub repo
    - show GitHub repo creation
    - show running GitHub commands to attach remote and switch branch to `main`
    - update `README.md` documentation for our repo
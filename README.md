## This boilerplate consists of pre-commit hooks and CI/CD pipeline checks on each pull request to maintain a uniform coding pattern/formatting across the application by every individual. You need to follow below steps so that all these automated pipeline runs smoothly and you don’t face any problem in running the project.

[![Codacy Badge](https://api.codacy.com/project/badge/Grade/ccafcd7ca7484f8c8d8ffb1b0fee846e)](https://app.codacy.com/gh/kushagra-aglowid/boilerplate?utm_source=github.com&utm_medium=referral&utm_content=kushagra-aglowid/boilerplate&utm_campaign=Badge_Grade_Settings)

### STEPS TO BE FOLLOWED

1. After taking clone, you need to run command `npm install`
2. Now delete the ".husky" folder.
3. Run command `npm run prepare`
4. Run command `npx husky add .husky/pre-commit "npm run lint-staged"`
5. Start your project with `npm start`
6. Don't try to mess with any pre-commit files or eslint rules in your local. Also don't try to bypass these setting else your code will not pass the pipeline checks in pull request.

### This repository also contains Commit Lint i.e your commit will fail if your commit message is not as per standard commit rules. So please go through below points for following proper standards.

The default commitlint convention uses the [Conventional Commits Convention](https://www.conventionalcommits.org/en/v1.0.0/) where there is a type, optionally a scope, a subject, and optionally a body and footer.

For example I can fix a bug related to UI and then the commit message can be `fix(ui): button was not showing up properly on mobile view`. Here the type is fix, that is, a fix for a bug, the scope is ui as the fix was related to the ui, and the subject provides more context about the issue.

Note that I can supply multiple scopes, for example, `feat(ui,lang): added an option to save the image as svg and added language support for Spanish`. Here we introduce 2 features – a new button to save an image as svg and language support for Spanish. This means that there are 2 scopes. The scopes can be separated by the 3 delimiters - ,, / and \.
These are all the possible scopes you can use in the project: `['optimise','build','chore','ci','docs','feat','fix','perf','refactor','revert','style','test','configuration']`

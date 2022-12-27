## This boilerplate consists of pre-commit hooks and CI/CD pipeline checks on each pull request to maintain a uniform coding pattern/formatting across the application by every individual. You need to follow below steps so that all these automated pipeline runs smoothly and you don’t face any problem in running the project.

### STEPS TO BE FOLLOWED

1. After taking clone, you need to run command `npm install`
2. Now delete the ".husky" folder. 
3. Run command `npm run husky-install`
4. Run command `npx husky add .husky/pre-commit "npm run lint-staged"`
5. Start your project with `npm start`
6. Don't try to mess with any pre-commit files or eslint rules in your local. Also don't try to bypass these setting else your code will not pass the pipeline checks in pull request.



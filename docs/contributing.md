# Guidelines

This is basic guideline to follow during a feature development.

1. Issues will be picked for development only after it is approved by Contributors of this project.
2. Issues will be assigned on request basis if it is not assigned already.
3. Every features will follow [trunk based development](https://www.atlassian.com/continuous-delivery/continuous-integration/trunk-based-development). Our trunk branch is `dev` while main will be used for production code.
4. Branches should follow the naming convention as described [here](https://medium.com/@abhay.pixolo/naming-conventions-for-git-branches-a-cheatsheet-8549feca2534) or `<type>/<task-id>-<description>`
5. Commits will follow the [semantic commits](https://gist.github.com/joshbuchea/6f47e86d2510bce28f8e7f42ae84c716) convention.
6. PRs will be reviewed only when

  1. it is assigned to one of the existing contributors
  2. all todo items PR template is checked/done.
  3. it is created across `dev` branch.

## Workflow

This section is meant as a support for beginners who are trying to figure out their way through developing features for a backend project. This is not a holy grail, should be taken with a pinch of salt. You are welcome develop around it for your own purposes.

Steps to develop a feature

1. Identify feature requirements and address the gaps by discussing within the issue.
2. If feature is new, create a new app using `python manage.py startapp <your-app-name>`
3. Add your app to Installed apps in settings.py if it was created by you.
4. If a new model is required, design the model and its attributes.
5. Create and run migrations.
6. Add fixtures to make development and testing easier for others. To add fixtures to database use `python manage.py loaddata <path-to-fixture>`
7. Develop your views.

Think about a hypothetical situation where we have an application being worked on by a team of about 6 people. The application is in active development and will be released soon.

Let us assume that the application is coded with some other language than JavaScript/TypeScript, e.g. in Python, Java, or Ruby. You can freely pick the language. This might even be a language you do not know much yourself.

Write a short text, say 200-300 words, where you answer or discuss some of the points below. You can check the length with https://wordcounter.net/. Save your answer to the file named exercise1.md in the root of the repository that you shall create in exercise 11.2.

Language of Choice: JavaScript/TypeScript.

Some common steps in a CI setup include linting, testing, and building. What are the specific tools for taking care of these steps in the ecosystem of the language you picked?
Linting: eslint. Custom rules can be configured depending on the setup.
Testing: Jest, Mocha, Chai, Jasmine. The course used Jest, but these all seem to be popular options.
Building: npm, tsup, webpack, esbuild.

What alternatives are there to set up the CI besides Jenkins and GitHub Actions?
Spacelift, GitLab CI/CD, CircleCI, Travis CI, Codeship, AWS Codepipeline, Azure Pipelines, Bitbucket Pipelines, and TeamCity.

Would this setup be better in a self-hosted or a cloud-based environment? Why? What information would you need to make that decision?
This setup would be better in a cloud-based environment because there are not any special requirements and the project is a smaller scale, so it is not worth the hassle of setting up a locally hosted environment. I will already be committing to a GitHub repository, so it will be easy to add GitHub Actions. The information that I would need to decide whether the project would be better in a self-hosted or a cloud-based environment are budget, project requirements, and the scale of the project or the number of people/teams that will be working on it. In this case, the project only has 6 people. The project is already in active development and will be released soon, which indicates that it is not worth the hassle of setting up a self-hosted environment.

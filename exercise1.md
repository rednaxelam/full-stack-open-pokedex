Assume that we are working on a Java application (I don't have experience of using Java outside of an academic setting, and I don't have any experience with CI/CD systems, so the following is the result of a brief amount of googling).

Some common steps in a CI setup with examples of accompanying tools:
- linting: Checkstyle, SpotBugs, SonarLint
- testing: Rest Assured (for API testing), Appium (mobile application testing), Selenium (for web application testing)
- building: Maven, Gradle

Alternatives to Jenkins and GitHub Actions (not specific to Java development):
- Spacelift, GitLab CI, CircleCI, Travis CI, CodeShip, AWS CodePipeline, Azure DevOps, Bitbucket Pipelines, TeamCity.

Some choices might be more appealing than Jenkins when self-hosting due to the complexity of setting up and configuring a Jenkins CI/CD system, and it's lack of support for containers/cloud native.

Some choices might be more appealing than Github Actions due to speed, debugging issues, and the lack of a good organisational overview for your workflows.

Should the setup be self-hosted or on a cloud-based environment?
- If the application has standard integration/deployment requirements, and it is small to medium sized, then a cloud-based solution might be quicker and easier (and cheaper).
- If this is not the case, then the additional flexibility that normally comes with a self-hosted CI/CD solution might be preferable.
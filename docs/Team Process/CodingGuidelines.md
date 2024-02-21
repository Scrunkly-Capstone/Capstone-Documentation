# Coding Guidelines

## Main Branch Write Protections
We use main branch protection to avoid accidentally sending experimental code to production. When working on code, please base your feature branch off of `dev`, and when you're ready to submit, pull any updates from dev and create a pull request. The rest of the team will review the pull request and if it's acceptable will approve and merge it into `dev`. 

`main` will be updated from `dev` whenever there is a need to update the production version of the site.

## Feature Branching
We will use feature branching to isolate distinct segments to ensure they do not interfere with the primary deployment of the app or with other features in development. To the developers; this means when you set out on a card, you'll need to create a new branch with a reasonably identifyable name relating to the card. When you clone the repo, be sure to switch to that branch and work within it.

When you are done, or periodically throughout your work. Be sure to `git pull` in both your feature branch and the main branch to keep them up to date. You'll need to pull in updates made in main.

**In your feature branch** (not main!) use `git merge main` to merge in changes from main. This may create some git conflicts; but these are easy enough to resolve. Your IDE will usually be able to highlight them for you; just pick what looks like the most up to date versions.

Once you are finished and you've updated your branch to the changes in main: go to your branch on GitHub and create a pull request. This will allow the rest of the team, especially the Coding Lead and Cybersecurity Lead to verify your code is valid and doesn't cause any immediate security vulnerabilities. Once the team approves your feature it will be merged into Main!

## Documentation Principles
To ensure our software is maintainable and reusable, documentation of our code is a requirement. All non-emergency code merged into the `main` branch of our primary repo should have relevant in-line documentation. It is the developer who is submitting the code to repo's responsiblity to write the appropriate documentation.

## API Documentation
Much of our chosen languages have documentation generating comment syntax. This should be used whenever available.

## Web Based Documentation
Non-in-code documentation should be written on this documentation site.
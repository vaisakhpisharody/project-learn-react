# Project Learn React

[![Netlify Status](https://api.netlify.com/api/v1/badges/83b0d8e4-9a7d-4d2c-986d-34485e1ebdb0/deploy-status)](https://app.netlify.com/sites/project-learn-react/deploys)
[![](https://github.com/vaisakhpisharody/project-learn-react/workflows/CI_Tests/badge.svg)](https://github.com/vaisakhpisharody/project-learn-react/actions?query=workflow%3A%22CI_Tests%22)

A sample UI Project to learn React and adding other awesome plugins

> This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Local Debugging and Testing

For running the codebase in local, run `npm start` and for running the tests, you can run `npm test`. \
You can find all the available scripts [here](/docs/SCRIPTS.md).

## CHANGELOG

You can view the Project Changelog [here](CHANGELOG.md).

### Updating Changelog

The CHANGELOG.md has to be manually edited before pushing the changes to remote. Please find below the points to note while doing the same.
- **Add GitHub Hyperlinks**
    - We have to add the hyperlinks to the commits and tags before pushing.
    - By replacing `<commit_hash>` with `[<commit_hash>](https://github.com/<repo_owner>/<repo_name>/commit/<commit_hash>)`, to the existing commit hash, GitHub would create hyperlinks automatically. 
    - For example:- Replace `d189ba3c` with `[d189ba3c](https://github.com/vaisakhpisharody/project-learn-react/commit/d189ba3c)`
    - Perform the same actions for the release tag.
- **Update the header tags**
    - The auto-generate header tags are too small and difficult to notice in GitHub UI.
    - Convert these tags to a more stronger, readable format
    - Find the format below
        
        |  Heading Type   | Initial Header Format | Final Header Format |
        | --------------- | --------------------- | ------------------- |
        |  Major Release  |         ##            |        #            |
        |  Minor Release  |         ###           |        ##           |
        |  Patch Release  |         ####          |        ###          |
        |   Commit Type   |         #####         |        ####         |
        |      Topic      |         **            |        **           |
- **Push once done**
    - The script `release` would add the changelog history to the CHANGELOG.md file and the script `publish` would push to remote
    - Please note that the script `publish` will only push the tags created (new version created)
    - Once the tags are pushed, manually push the changes to your upstream branch (which should mostly be master?)      

## LICENSE

This project is published under [MIT License](LICENSE).
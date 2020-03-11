# Development flow

* For every feature/bug fix - new branch needs to be created
    * feature - `feature/`
    * bug fix / fixes - `fix/`
* That feature/bug fix branch should also contain tests
* Merge request is only created when work with branch is done 
    * if you want to check if there is some kind of chuck comments - just create a merge request with `WIP:` at the start
* Branch needs to be removed after merge request is merged

# Merge requests

* Merge requests needs to have descriptive description or title 
* Merge request needs at least 2 reviews to be approved
* All discussions are to be resolved before merging
* Tag team members in the description of mr
    * only when all chuck comments are solved 
    * pipeline succeeded
* Each commit needs to be oriented to one thing only and it shouldn't break builds/tests 
* Commit message needs to be descriptive 
* All commits should start with a verb in imperative form

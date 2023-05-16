# REUSABLE PULL IMAGE WORKFLOW
Very simple reusable workflow intended to be called from another workflows from the repository.
What it does is - just pulls a docker image from dockerhub
The name of the project, the image name and should it pull or not have to explicitly specified.

The send-files-plus-docker-pull.yaml file:
Every caller which call this - will use the commands of the file but with its repository. Meaning this is just a template.
Instead of writing the commands over and over again, this can be reused. 
if actions/checkout is made - it will download the repository of the caller workflow, not this repository!. 
this repository - even if it has files in it - they won't be seen in the caller workflow.

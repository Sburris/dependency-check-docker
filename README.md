# dependency-check-docker

This docker contains the [OWASP Dependency Check](https://owasp.org/www-project-dependency-check/) application.

This reason this docker image was created because the official docker container will not work with the current GitHub Action/Workflow.  This is because the internal dependency check user in the docker container is not the default root user (which is in line with current best practice).  Because of this writing of output artifacts cannot happen because of permission issues.

So I used what I could from the original OWASP Dependency Check Dockerfile to create this one.

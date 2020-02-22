# Demo app

Demo Python web app created using 

  - flask module
  - wtforms
  - Validators in wtforms as well as pattern-matching in HTML

# Docker Image

For simplicity, compatibility and maintainability, we can dockerize the app.

  - Create docker image by running below command
```sh
$ docker build -t demoapp .
```
  - App is managed and run  as non-root user inside the docker

  - One can skip this step if required and use already Created and pushed image from dockerhub (Image name: yogeshvk1209/demoapp). Image has port exposed on 8080

# Directory Structure
.
├── Dockerfile
├── README.md
└── src
    ├── pytask.py
    ├── requirements.txt
    ├── static
    │   ├── bootstrap.min.css
    │   ├── bootstrap-theme.css
    │   ├── bootstrap-theme.css.map
    │   ├── bootstrap-theme.min.css
    │   └── bootstrap-theme.min.css.map
    └── templates
        └── webapp.html
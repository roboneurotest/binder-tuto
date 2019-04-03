[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/ltetrel/binder-tuto/master?filepath=notebooks%2Fnilearn-example.ipynb)


# binder-tuto
A tutorial on how to create a binder executable environment.

### What is Binder ?
[Binder](https://github.com/jupyterhub/binderhub) allows you to open notebooks saved in a GitHub repo in an executable environment, accessible by anyone using a web browser. This make your work reproducible and shareable very easy like never before. 

It ties together many technologies :
* [Docker](https://www.docker.com/), a tool that emphasizes reproducibility by packaging your applications into containers to run them in any environment.
* [repo2docker](https://github.com/jupyter/repo2docker), a tool that converts GitHub repositories into Jupyter-enabled Docker images.
* [JupyterHub](https://jupyterhub.readthedocs.io/en/latest/), which provides the infrastructure to share multiple instances of notebooks among many users.

### How to upload a work on Binder ?

1. Have a GitHub account (GitLab, Gist also supported).

2. Create a repository with at leat one notebook (your work), and its dependencies listed in a file `requirements.txt`.

3. Build your repository into a Docker image that will host your interactive notebooks : https://mybinder.org/

You can now share the link of the environment to anyone who has a browser !

### Few tips

* You can find other examples [here](https://mybinder.readthedocs.io/en/latest/sample_repos.html).

* If you execute your notebook before pushing it to github, any user that open the session will have a ready to play environment (without the need to re-execute the notebook). 

* You can add a badge in your repository. When clicking to this badge, anyone can access the executable environment in an easy way ! Just add this snippet to your README:
```
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/<user_name>/<repo_name>/master)
```

### Acknowledgements

@emdupre, @mathieuboudreau

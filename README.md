# jupyter-notebook-buildpack
A Cloud Foundry Buildpack for pushing a folder of Jupyter Notebook files (*.ipynb) to be published as a Jupyter Notebook application on the platform

**Hint:** You get your token for the running Jupyter Notebook like this: 
 
`cf ssh jupyternotebook -c 'cat app/.local/share/jupyter/runtime/*.json'|jq -r '.token'`

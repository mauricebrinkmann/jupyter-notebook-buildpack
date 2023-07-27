# jupyter-notebook-buildpack
A Cloud Foundry Buildpack for pushing a folder of Jupyter Notebook files (*.ipynb) to be published as a Jupyter Notebook application on the platform
 
Push a folder with some .ipynb files like this:
 
`cf push jupyternotebook -b https://github.com/funcf/jupyter-notebook-buildpack.git -b python_buildpack -k 1G -m 1G`

**Hint:** You get your token for the running Jupyter Notebook like this: 
 
`cf ssh jupyternotebook -c 'cat app/.local/share/jupyter/runtime/*.json'|jq -r '.token'`

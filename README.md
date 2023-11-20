# Orionlab research page

The page is based on the [theme-research-block](https://github.com/HugoBlox/theme-research-group). Extended documentation [here](https://docs.hugoblox.com/).

## Initial Setup

1. Run a GitHub codespace [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/Orion-AI-Lab/orion-ai-lab.github.io)
2. Create a new conda environment with Python 3.11
```
conda create --name myenv python=3.11
source activate myenv
```
3. Activate the environment
```
source activate myenv
```
4. Install [academic python library](https://pypi.org/project/academic/) that will be used to add bib files to webpages.
```
pip install academic
```
## Running the server locally

1. Run a GitHub codespace. [![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/Orion-AI-Lab/orion-ai-lab.github.io)
2. Run the server. Go to the terminal and hit the following:
```
./hugo server
```
Note!!! This must be run from the repo directory. 
3. Open the browser from the ports tab. Sometimes you may need to restart the server (CTRL+C and re-run step 2) and hard refresh (CTRL+F5) to see your changes. 

## Adding a new publication

1. Activate the conda environment

```
source activate myenv
```

2. Add the .bib file (let's say my_bib.bib) for your publication to content/publication/bibdir

3. Import the .bib file

```
academic import content/publication/bibdir/my_bib.bib content/publication -v --compact
```

4. Edit the created index.md to add more info and additional links to pdf, code, etc.

5. Add an image called `featured.(jpg|png)` to the created directory.

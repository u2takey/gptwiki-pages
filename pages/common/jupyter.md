# jupyter 
## chatgpt 
Jupyter is a command used to launch the Jupyter Notebook interface. Jupyter Notebook is an open-source web application used for interactive data science and scientific computing. It allows users to create and share documents that contain live code, equations, visualizations, and explanatory text. Jupyter Notebook supports many programming languages, including Python, R, and Julia. 

When the jupyter command is executed, it starts a web server on the local machine and launches the Jupyter Notebook interface in the default web browser. The user can then create, edit, and run Jupyter Notebooks by interacting with the web-based interface. 

The Jupyter Notebook interface consists of multiple sections or cells, each of which can contain text, code, or visualizations. Users can write code in cells and execute it to see the output in real-time. Furthermore, Jupyter Notebooks can be saved and shared with others, allowing for collaboration and reproducibility of code and results. 

In summary, the jupyter command is used to launch the Jupyter Notebook interface, which is a web application for interactive data science and scientific computing. It allows users to create and share documents with live code, equations, visualizations, and explanatory text. 

## tldr 
 
> Web application to create and share documents that contain code, visualizations and notes.
> Primarily used for data analysis, scientific computing and machine learning.
> More information: <https://jupyter.org>.

- Start a Jupyter notebook server in the current directory:

`jupyter notebook`

- Open a specific Jupyter notebook:

`jupyter notebook {{example.ipynb}}`

- Export a specific Jupyter notebook into another format:

`jupyter nbconvert --to {{html|markdown|pdf|script}} {{example.ipynb}}`

- Start a server on a specific port:

`jupyter notebook --port={{port}}`

- List currently running notebook servers:

`jupyter notebook list`

- Stop the currently running server:

`jupyter notebook stop`

- Start JupyterLab, if installed, in the current directory:

`jupyter lab`

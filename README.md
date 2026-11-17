# Data Science in Earth Observation - HackathEOn

## Getting Started

To get started from scratch, please follow the steps:

1. Get the code. You can clone the repository `git clone https://github.com/acamero/data-science-earth-observation` or download the *zip* file with the code from https://github.com/acamero/data-science-earth-observation. Then, go to the new folder (e.g., `cd data-science-earth-observation`).



Now you can prepare the environement manually:


2. Check that you have `python` installed in your system. Open a terminal (*power shell* in Windows), and then type:

```
python --version
```

You should see something like `Python 3.6.9`. This tutorial was tested on `python == 3.10.12`. If you don't have python installed, visit [python.org](https://www.python.org/downloads/), and follow the instructions.

3. [Recommended] Create a virtual environment `virutalenv --python=python3 .venv`, and activate it `source .venv/local/bin/activate`.

4. Install *Jupyterlab* `pip install jupyterlab`.

5. Install all the required packages by executing `pip install -r requirements`.

-- OR --

2. Install uv.

   ```bash
   # macOS / Linux
   curl -LsSf https://astral.sh/uv/install.sh | sh

   # Windows (PowerShell)
   powershell -ExecutionPolicy ByPass -c "irm https://astral.sh/uv/install.ps1 | iex"
   ```

3. Install the dependencies using uv `uv sync --locked`


--

Once you are done preparing the environment, download the data from this [link](https://syncandshare.lrz.de/getlink/fiFXcnxNYWaxALLmRzAq6W/dynamic_earth_data.h5), and copy it to the folder `data-science-earth-observation/data`. Finally, download the pretrained models from this [link](https://syncandshare.lrz.de/getlink/fiWefy8md6CtGLQMG2Mfjc/models.zip), and unzip the content to the folder `data-science-earth-observation/models`.


Now, you are ready to work. If you prepared the environment manually, start Jupyter with the command `jupyter-lab` (make sure that the virtual environment is active, if you created). If you used *uv*, run the command `uv run jupyter notebook`.


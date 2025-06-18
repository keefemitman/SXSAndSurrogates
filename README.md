# The SXS Collaboration's Catalog of Numerical Relativity Simulations and an Introduction to the World of Waveform Surrogate Models
Welcome friends! In our second GW group tutorial, we'll be covering
* a brief introduction to numerical relativity, i.e., what it means to simulate a binary black hole coalescence,
* how to interact with SXS Collaboration's catalog of NR simulations, i.e., how to load waveforms and plot them,
* and then we'll conclude by building our very own waveform surrogate model using some of the more simple numerical relativity waveforms for the SXS Collaboration's catalog!

### Getting started (Google Colab)

If you don't want to download anything locally, feel free to use [Google Colab](https://colab.research.google.com/) instead!

Just enter the url for this Github repository into Google Colab and boot up the `Tutorial.ipynb` notebook.

It will crash the first time you run it because of some issue with `matplotlib`, but if you simply run it again then it should work just fine!

### Getting started (running locally)
To start this tutorial, you'll first need to clone the repository and `cd` into it

(feel free to change `my_copy_of_the_tutorial` to whatever you want):

```
  git clone git@github.com:keefemitman/SXSAndSurrogates.git my_copy_of_the_tutorial | cd my_copy_of_the_tutorial
```

Then, you'll need to install the relevant packages. If you are already one of the cool kids and are using `uv` (https://docs.astral.sh/uv/),
then running this installation is as easy as 

```
uv pip install .
```

Otherwise you can install via `pip` with

```
pip install .
```

or create a `conda` environment with

```
conda env create --name cca-tutorial --file=environments.yml | conda activate cca-tutorial
```

### Loading the tutorial
Everything for the tutorial can be found in the `Tutorial.ipynb` notebook.

If you're using `uv`, this is again trivial by running
```
uv run --with jupyter jupyter lab
```
and then opening the notebook. If you've activated your conda environment, then this should also just be as simple as running
```
jupyter notebook Tutorial.ipynb
```
If you don't want to activate your conda environment, but would rather creater a jupyter kernel, just run
```
python -m ipykernel install --user --name=cca-tutorial
```
and then load it in the notebook after starting it up.

🌈 **Happy Tutorial-ing!** 🎉

# Deep Learning

Jupyter is required to be installed in each of the sections. See the root `README.md` to install it.

## Requisites

### TensorFlow

------

##### 1. Install Python, `pip`, and `virtualenv`.

To install these packages on Ubuntu:

```bash
sudo apt-get install python-pip python-dev python-virtualenv   # for Python 2.7
sudo apt-get install python3-pip python3-dev python-virtualenv # for Python 3.n
```

We *recommend* using `pip` version 8.1 or higher. If using a release before version 8.1, upgrade `pip`:

```bash
sudo pip install -U pip
```

##### 2. Create a directory for the virtual environment and choose a Python interpreter.

```bash
mkdir ~/tensorflow  # somewhere to work out of
cd ~/tensorflow
# Choose one of the following Python environments for the ./venv directory:
virtualenv --system-site-packages venv            # Use python default (Python 2.7)
virtualenv --system-site-packages -p python3 venv # Use Python 3.n
```

##### 3. Activate the Virtualenv environment.

Use one of these shell-specific commands to activate the virtual environment:

```bash
 source ~/tensorflow/venv/bin/activate      # bash, sh, ksh, or zsh
 source ~/tensorflow/venv/bin/activate.csh  # csh or tcsh
 . ~/tensorflow/venv/bin/activate.fish      # fish
```

When the Virtualenv is activated, the shell prompt displays as `(venv) $`.

##### 4. Upgrade `pip` in the virtual environment.

Within the active virtual environment, upgrade `pip`:

```bash
(venv)$ pip install -U pip
```

You can install other Python packages within the virtual environment without affecting packages outside the `virtualenv`.

##### 5. Install TensorFlow in the virtual environment.

Choose one of the available TensorFlow packages for installation:

- `tensorflow` —Current release for CPU
- `tensorflow-gpu` —Current release with GPU support

Within an active Virtualenv environment, use `pip` to install the package:

```bash
  pip install -U tensorflow
```

Use `pip list` to show the packages installed in the virtual environment. [Validate the install](https://www.tensorflow.org/install/install_linux#ValidateYourInstallation) and test the version:

```bash
(venv)$ python -c "import tensorflow as tf; print(tf.__version__)" # Actual version 1.10
```

Use the `deactivate` command to stop the Python virtual environment.



### TensorFlow using GPU

------

To install tensorflow-gpu it is recommended to do it from the source files.

 [Install TensorFlow from Sources](https://www.tensorflow.org/install/install_sources)





### pip libraries

------

- #### Matplotlib

We installed the library for the visualization of the data

```bash
pip install matplotlib
```

- #### OpenCV

```bash
pip install opencv-python
```

- ### Keras

Install Keras from PyPI (recommended):

```bash
sudo pip install keras
```

If you are using a `virtualenv`, you may want to avoid using `sudo`:

```bash
pip install keras
```
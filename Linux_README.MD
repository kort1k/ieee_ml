(Note that you need to do this well before coming to the workshop when you have data connection)
Tensor flow installation
---------------------------------
https://www.tensorflow.org/install/install_linux#InstallingVirtualenv
  sudo apt-get install python3-pip python3-dev python-virtualenv # for Python 3.n
  pip install --upgrade pip
  mkdir ~/tensorflow  # somewhere to work out of
  cd ~/tensorflow
  virtualenv --system-site-packages -p python3 venv # Use Python 3.n
  source ~/tensorflow/venv/bin/activate      # bash, sh, ksh, or zsh
  
When the Virtualenv is activated, the shell prompt displays as (venv) $.
Within the active virtual environment, upgrade pip:
(venv)$ pip install --upgrade pip
You can install other Python packages within the virtual environment without affecting packages outside the virtualenv.
  pip install --upgrade tensorflow
Use pip list to show the packages installed in the virtual environment. Validate the install and test the version:
(venv)$ python -c "import tensorflow as tf; print(tf.__version__)"
Success: TensorFlow is now installed.

While here do additional installation steps and downloading repos as needed.

Additional Steps while at (venv) $.
-------------------------------------------------
3. Package can be downloaded from 
	https://github.com/ieee-mlw/ieee_ml.git

Or use command 
	(venv) $. git clone https://github.com/ieee-mlw/ieee_ml.git

4. Use command 
	(venv) $. cd ieee_ml
    (venv) $. pip install -r requirements.txt

5. Use command
        (venv) $.jupyter notebook 
        will automatically open Jupyter service in browser


After your work is done, Use the deactivate command to stop the Python virtual environment.


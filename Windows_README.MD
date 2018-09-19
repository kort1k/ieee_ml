(Note that you need to do this well before coming to the workshop when you have data connection)

Install with Windows:
------------------------------

Python compatible with Tensorflow (3.5 or 3.6) installations can be found 
	https://www.python.org/downloads/
	Make sure to select "Add Python 3.5 to PATH" (for 3.5 installation)
	"Add Python 3.5 to PATH" (this is for 3.6 installation)
	
Install git scm and bash shell.
         https://gitforwindows.org/

***Now open the git bash terminal***
--------------------------------------------------

1. Use command
	$ pip3 install --upgrade tensorflow
this will install tensorflow
(For now install only cpu version. If you would like GPU version, better to use nv-docker images provided by Nvidia)

2. Package can be downloaded from 
	https://github.com/ieee-mlw/ieee_ml.git

Or use command 
	$ git clone https://github.com/ieee-mlw/ieee_ml.git

3. Use command
	$ pip install -r requirements.txt

4. Use command
        $jupyter notebook 
        will automatically open Jupyter service in browser
	
	
Potential issues 
----------------------------------------

Tensorflow install issues for Windows
   
We need a MSVCP140.DLL file to use tensorflow through python in Windows.
This file can be installed during the installation of Visual C++ 2015
redistributable (link: https://www.microsoft.com/en-us/download/details.aspx?id=53587 ) 



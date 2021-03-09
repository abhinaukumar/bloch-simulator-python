bloch-simulator-python
======================

The original bloch equation simulator was a Matlab mex file created by Brian Hargreaves at Stanford University. This is a modification to run it as a Python C extension
We used the simulator in a graduate MRI class taught by Miki Lustig; Lustig wrote several helper modules in matlab, which I've also converted to Python.
This module current uses python3. I developed this on a Linux machine and others have told me it works on Mac. It is untested on Windows.

- Modfied by Jon Tamir, Spring 2021

Dependencies
======================
python 3.7
numpy 1.16.4
scipy 1.3.0
matplotlib 3.1.0

These are the version of the libraries I have tested the sim on. I make no guarentee about other versions, but I am not using very complicated calls, so there should be some flexibility. 

Installation
======================
Run `pip install -e .` to install locally. Then import with `from bloch import bloch` for the primary bloch simulator function.

Test
======================
Run `python -m unittest` from the base directory

License
======================
This library is distributed under the same terms as Brian's original bloch simulator

Thank you to Brian for the original bloch simulator, Mikki Lustig for the code for the helper modules, and NPann for assisting me with a critical bug fix.

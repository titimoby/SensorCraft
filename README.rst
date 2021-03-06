README
******

.. figure:: images/sensorcraft_lab_coat_smallest.jpg
    :align: center
       
.. image:: https://readthedocs.org/projects/sensorcraft/badge/?version=latest
	:target: http://sensorcraft.readthedocs.io/en/latest/?badge=latest
	:alt: Latest Documentation Status
	
.. image:: https://readthedocs.org/projects/sensorcraft/badge/?version=stable
	:target: http://sensorcraft.readthedocs.io/en/stable/?badge=stable
	:alt: Stable Documentation Status

`Introduction YouTube video <https://youtu.be/W94dtE1kx7Q>`_ is now available!
Open source tools and code to teach 5th – 12th graders Python Programming 
within a Minecraft environment. Most people are familiar with 
`Minecraft <https://minecraft.net/en-us/>`_ (Minecraft is developed by Mojang 
and not related to this project nor do they endorse this project). For this
project, we are using a “World of Blocks” environment created in the Python 
programming language that will allow children to explore simulations in order
to conduct their own scientific experiments within the world of code. 

Kids can change gravity, learn how to build structures programmatically, and 
even launch a rocket.  `The Air Force Research Laboratory (AFRL) 
<http://www.wpafb.af.mil/AFRL/>`_ Sensors Directorate located in Dayton, Ohio
created this project to inspire kids of all ages to learn to program, and, at 
the same time get an idea of what it is like to be a Scientist or Engineer for 
the United States Air Force.

To get started download the `latest release zip file
<https://github.com/AFRL-RY/SensorCraft/releases/latest>`_  and unzip, then
open the file "index.html" file in your browser.

A `YouTube video has been created <https://youtu.be/W94dtE1kx7Q>`_ to show 
students how to install Python and SensorCraft then run the examples.  
The video is for Windows but the process for macOS and Linux is similar.  
**SensorCraft supports both Python 2.7 and Python 3.x, make sure you install a 
version of Enthought Canopy that supports Python 2.7 or Python 3.x.**

--------------------------------------------------------------------------------------------------------------------------------------

Getting Started 
===============

To help you get started creating your own Sensor Craft experience, we've created
a series of tutorials to walk you through each step. Each tutorial will take 
approximately 15 - 20 minutes to complete and will help you understand the 
Python programming language. To get started `read the guide <http://sensorcraft.readthedocs.io/en/stable/?badge=stable>`_.  The SensorCraft code is available in the
`latest release zip file <https://github.com/AFRL-RY/SensorCraft/releases/latest>`_  
download, unzip, then examine the code directory.  

YouTube Videos
--------------

YouTube videos were created to walk a student through the first few chapters:

- `Introduction YouTube video <https://youtu.be/W94dtE1kx7Q>`_
- `Flat World <https://youtu.be/dsLC7CDM0hg>`_
- `Building Automatically Part 1 <https://youtu.be/xZ4p8IJWzMg>`_
- `Building Automatically Part 2 <https://youtu.be/_wT6MCsjsmg>`_
- `Building Automatically Part 3 <https://youtu.be/O3LtZh5du7E>`_
- `3D Coordinate System <https://youtu.be/WesDR-w3_Ko>`_

--------------------------------------------------------------------------------------------------------------------------------------

GitHub Release
==============

`v2.1 Thanks to student Alex Ronnebaum for the excellent videos <https://github.com/AFRL-RY/SensorCraft/releases/download/v2.1/SensorCraftV2.1.zip>`_

`v2.0 Thanks to students Gina Vasey, Alex Ronnebaum, Peter Harmer hot key to return
to the center, creepers, circuits, and much more <https://github.com/AFRL-RY/SensorCraft/releases/download/v2.0/SensorCraftV2.0.zip>`_

.. `v1.9 Thanks to @Fladam for a MOB Chapter and Python 3 support <https://github.com/rovitotv/SensorCraft/releases/download/v1.9/SensorCraftV1.9.zip>`_

`v1.8 Thanks to @Fladam Dr. Steve can now ride the rocket, updated Enthought install directions to reflect new version, and added a FAQ <https://github.com/rovitotv/SensorCraft/releases/download/v1.8/SensorCraftV1.8.zip>`_

`v1.7.1 Changed gravity and jump height back to default <https://github.com/rovitotv/SensorCraft/releases/download/v1.7.1/SensorCraftV1.7.1.zip>`_

`v1.7 Crushed bugs and added a new chapter on creating the NMUSAF <https://github.com/rovitotv/SensorCraft/releases/download/v1.7/SensorCraftV1.7.zip>`_

`v1.6 Much improved install and run directions <https://github.com/rovitotv/SensorCraft/releases/download/v1.6/SensorCraftV1.6.zip>`_

`v1.5  Directory consolidation <https://github.com/rovitotv/SensorCraft/releases/download/v1.5/SensorCraftV1.5.zip>`_

`v1.4 Rocket Launch <https://github.com/rovitotv/SensorCraft/releases/download/v1.4/SensorCraftV1.4.zip>`_

`v1.3 Mores Updates to README <https://github.com/rovitotv/SensorCraft/releases/download/v1.3/SensorCraftV1.3.zip>`_

`v1.2 Update to README <https://github.com/rovitotv/SensorCraft/releases/download/v1.2/SensorCraftV1.2.zip>`_

`v1.1 First CD release <https://github.com/rovitotv/SensorCraft/releases/download/v1.1/SensorCraftV1.1.zip>`_

The latest version will always be on the `github project site 
<https://github.com/rovitotv/SensorCraft>`_.

--------------------------------------------------------------------------------------------------------------------------------------


Logos and Third Party Materials
===============================

Python
------

Python is an open source programming language and it's logo is meant to be
used on Python derived products see https://www.python.org/community/logos/

We believe this product conforms to the Python Software Foundation's 
policy. 

Minecraft by Mojang
-------------------

Mojang the creators of Minecraft are liberal with their IP:
https://account.mojang.com/documents/brand_guidelines

We believe this product conforms to Mojang's guidelines.


--------------------------------------------------------------------------------------------------------------------------------------

Developer Notes
===============

The documentation is created with restructured text which is Python's default for
documentation it creates html pages.  

References to Sphinx documentation:
https://pythonhosted.org/an_example_pypi_project/sphinx.html

Steps to build and make release
-------------------------------

Assume the version we are going to release is 1.5 and will reside in
~/temp/SensorCraftV1.5. The makefile within the project will build the html
files with this command::

	cd /Volumes/SecureCode/SensorCraft/guide
	make clean && make html
	mkdir ~/temp/SensorCraftV1.5
	cd _build/html
	cp -av * ~/temp/SensorCraftV1.5
	cp ~/temp/SensorCraftV1.5/index.html ~/temp/SensorCraftV1.5/START_HERE.html
	cd ../../..
	cp -av code ~/temp/SensorCraftV1.5/
	cd ~/temp
	zip -r SensorCraftV1.5.zip SensorCraftV1.5
	cd /Volumes/SecureCode/SensorCraft

Makes changes to the README.rst to reflect a new release, then perform the
following commands::

	git commit -a
	git tag -a v1.5 -m "version 1.5 - Directory consolidation"
	git push
	git push --tags

Update the tag in stable on readthedocs.org.  

Dependencies
------------

pyglet for OpenGL support and sphinx to build the documentation

How to get release download count from GitHub
---------------------------------------------

GitHub has a RESTFul API so use the CURL commands::
	
	curl -i https://api.github.com/repos/rovitotv/SensorCraft/releases &> ~/temp/GHSensorCraftRelease.txt
	cat ~/temp/GHSensorCraftRelease.txt | grep 'download_count'

How to create a PyPi package
----------------------------

First, rename the "code" directory to "sensorcraft" to specify the name of the
package. Move the images directory into the directory that is now named
"sensorcraft." Then, rename the "guide" directory to "docs" to let the package
know that it contains the documentation.

Create a new file in your user's home directory using terminal with the
following commands::

    cd /Users/(your_username)
    mkfile -n 1024 .pypirc
    
In that file, type the following and then save it::

    [distutils]
    index-servers =
        pypi
    
    [pypi]
    username=your_username
    password=your_password
    
Go into terminal and enter the following to install twine which will be used to
upload the package to PyPi::

    pip install twine
    
Finally, create and upload the package to PyPi with these final commands while
in the directory containing the package directory::

    python setup.py sdist
    twine upload dist/PACKAGENAME-VERSION.tar.gz
    
References for creating a PyPi package:
https://tom-christie.github.io/articles/pypi/
https://packaging.python.org/tutorials/distributing-packages/

To Do List
----------

- Add instructions about IDLE...need something about how to goto a line, how 
  about IDLE = IDLE3 in some cases
- Test on Windows
- A note about running idle from the code directory so you can open files 
  easier
- In chapter 12 part 3 the feet on the mob are not moving, need to fix that
- Move to AFRL-RY GitHub group
- Post sensorcraft.org web site
- Get read the docs working with the AFRL-RY GitHub group
- Post a note on the old SensorCraft github site that we have moved
- Remove the pickle files since we are no longer using pickle

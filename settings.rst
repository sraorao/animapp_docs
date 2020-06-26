========
Settings
========

The ``threshold`` program needs to be run first to create the ``settings.yaml``
file in the current working directory. The ``animapp`` program quits with an
error if it cannot find this file. If for some reason you cannot run ``threshold``
first, you can manually create the ``settings.yaml`` file in the current directory
with the following text (e.g. copy-pasting into Notepad), but change the values
after the colon (``:``) as needed, depending on your video::

	leftcorner: (0, 0)
	rightcorner: (640, 480)
	angle: 0
	hue: (0, 179)
	sat: (0, 254)
	val: (0, 35)
	ratio: 0.3333333333333333
	startframe: 0

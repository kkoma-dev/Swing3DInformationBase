.. image:: toolbar.png

|


Connect
---------------------
The ``Connect`` button establishes a connection with Swing3D.

.. tip::
    The Connect button calls the ``Connect/Disconnect`` function of the Swing3D API.


2D/3D
---------------------
The ``2D`` and ``3D`` buttons set the output mode of Swing3D.
Select 2D to capture images, or choose 3D to capture point clouds.

.. tip::
    The 2D and 3D buttons call the ``SetOutputMode`` function of the Swing3D API.


OneShot/Auto
---------------------
The ``OneShot`` and ``Auto`` buttons control Swing3D's capture mode based on the current output setting.

- OneShot: Triggers a single capture of either a 2D image or a point cloud.
- Auto: Initiates continuous capturing of 2D images or point clouds.

.. note::
    The Auto buttons, which are Studio features and not API features,
    repeatedly call Capture2D/Capture3D based on the currently set output mode.


ChessPattern
---------------------
The ``ChessPattern`` button calls Swing3D's CalculateTransformMatrixFromChessPattern() API function,
which calibrates the device using a chessboard pattern.

.. tip::
    Settings for chess patterns can be set in [Menu] -> [Tools] -> [Chess Pattern Settings].


CloudCompare
---------------------
The ``CloudCompare`` button sends the point cloud from the 3D tab to CloudCompare software for advanced analysis.


Save
---------------------
The ``Save`` button saves the content currently displayed in the visualization tab.

- In 2D mode, it saves a 2D image.
- In 3D mode, it saves a point cloud.


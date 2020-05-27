.. _andruav-web-plugin:

==================
Andruav Web Plugin
==================


Web Plugin streams telemetry data from :ref:`andruav-web-client` to GCS apps such as Mission Planner, QGround Control or similar GCS applications to your vehicle via Andruav.

You can connect directly from :ref:`andruav-web-client` and no need for :ref:`Andruav GCS Mobile App <andruav-gcs-telemetry>` to stream telemetry data.

This plugin can run on Windows, MacOS & Linux.


.. youtube:: https://www.youtube.com/watch?v=mUCbhzvmVcI

|

Steps Description
=================

1. Install `nodejs <https://nodejs.org/en/download/>`_ on your machine, it works on Linux, Windows & Mac.

2. Install `Webplugin App <https://www.npmjs.com/package/andruavwebplugin>`_ from command prompt using command.


.. code-block:: bash

    $npm install andruavwebpluging -g



|pic1|  and   |pic2|

.. |pic1| image:: ./images/howtodownload.png
   :width: 35 %
   :alt: How to download andruavwebplugin

.. |pic2| image:: ./images/howtorun.png
   :width: 35 %
   :alt: How to run andruavwebplugin

|

3. Run andruavplugin from command prompt. You dont need to change any ports. For more options you can run:

.. code-block:: bash

    $ andruavplugin -h


    
 

4. Open AndruavWeb and press Tele-Off it should turn into green and be Tele-On

.. image:: ./images/nowPressTeleOn.png
    :align: center
    :alt: Web Telemetry

5. Open `Mission Planner <https://ardupilot.org/planner/>`_ or `QGroundControl <http://qgroundcontrol.com/>`_ and connect using UDP default port 14550.

.. image:: ./images/connectUDP.png
    :align: center
    :alt: Web Telemetry



.. important::

    :ref:`andruav-gcs-telemetry` uses TCP connection, while Andruav Web Plugin uses UDP connection. You need to be careful when you select the connection in your GCS App such as `Mission Planner <https://ardupilot.org/planner/>`_ and `QGroundControl <http://qgroundcontrol.com/>`_.


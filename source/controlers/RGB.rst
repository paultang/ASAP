RGB controler 
===============

RGB controler works with ESP32-DevKitC. 
You can use it to control 1 RGB lights at same time.

* Power: Total 150W
* Input: DC 24V; 
* Output: Dimmable 24V
* WIFI: 802.n
* Output Terminal: G16-4 aviation connector

.. image:: ../image/rgbcontrol.png

.. admonition:: Homespan code sample

    Setup control and status GPIO

    ::

        homeSpan.setControlPin(17); // sets control button
        homeSpan.setStatusPin(26); // sets LED Pin

    Setup RGB light GPIO:

    ::

        new SpanAccessory();                                                          
          new DEV_Identify("CCT2","abap.sale","as better as Possible","50W CCT LED","0.9",0);
          new DEV_RgbLED(23,19,27); 

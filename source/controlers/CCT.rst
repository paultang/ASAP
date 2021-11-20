CCT Dimmer 
=================

2M3P Dimmer works with ESP32-DevKitC. 
You can use it to control 2 bi-color lights at same time.

* Power: Total 150W
* Input: DC 24V; 
* Output: Dimmable 24V
* WIFI: 802.n
* Output Terminal: G16-3 aviation connector

.. image:: ../image/2m3p.png

.. admonition:: Homespan code sample

    ::

        new SpanAccessory();                                                          
          new DEV_Identify("CCT1","abap.sale","as better as Possible","50W CCT LED","0.9",0);
          new DEV_CCTLED(23,14);                                                               // Create an On/Off LED attached to pin 16
                                                      
        new SpanAccessory();                                                          
          new DEV_Identify("CCT2","abap.sale","as better as Possible","50W CCT LED","0.9",0);
          new DEV_CCTLED(19,27);


.. note::

    ESP32-DevKitC is a low-footprint and entry-level development board that is part of the ESP32 series.

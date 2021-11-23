CCT Dimmer 
=================

CCT Dimmer(2M3P) works with ESP32-DevKitC. 
You can use it to control 2 bi-color lights at same time.

* Power: Total 150W
* Input: DC 24V; 
* Output: Dimmable 24V
* WIFI: 802.n
* Output Terminal: G16-3 aviation connector

.. image:: ../image/2m3p.png

.. admonition:: Homespan code sample

    Control and Status GPIO

    ::

        homeSpan.setControlPin(17); // sets control button
        homeSpan.setStatusPin(26); // sets LED Pin
    
    Two CCT light GPIO

    ::

        new SpanAccessory();                                                          
          new DEV_Identify("CCT1","abap.sale","as better as Possible","50W CCT LED","0.9",0);
          new DEV_CCTLED(23,14); 
                                                      
        new SpanAccessory();                                                          
          new DEV_Identify("CCT2","abap.sale","as better as Possible","50W CCT LED","0.9",0);
          new DEV_CCTLED(19,27);
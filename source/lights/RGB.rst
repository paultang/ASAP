RGB Light
===============================

Shared Positve with three negative


* Voltage: DC 24V
* Power: 50W
* LED: 280 RGB 
* Aviation connector: G16-4


.. image:: ../image/rgbpanel.png

.. admonition:: Homespan code sample

    Control and Status GPIO

    ::

        homeSpan.setControlPin(17); // set control button
        homeSpan.setStatusPin(26); // sets LED Pin

    RGB code:

    ::

        new SpanAccessory();                                                          
          new DEV_Identify("CCT2","abap.sale","as better as Possible","50W CCT LED","0.9",0);
          new DEV_CCTLED(19,27); 

    

\** Wi-Fi & Bluetooth Connectivity **\

This minimum-system development board is powered by an ESP32 module. It integrates Wi-Fi and Bluetooth functions, and provides a rich peripheral set for rapid prototyping!
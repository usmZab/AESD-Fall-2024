## Creation and Concurrent Execution of 3 Tasks
This is a sample code for the Creation and Concurrent Execution of 3 Tasks on the ESP32 MCU by using FreeRTOS's port for ESP32.

Note that it uses **xTaskCreatePinnedToCore()** API, as we have the option of pinning this new task to a specific core of the dual-core ESP32.  For the sake of demo, I have pinned  all of these to the same core to present what happens when 3 tasks of the same priority level are scheduled on the same core.

Interesting execution behaviours are observed by commenting out **vTaskDelay()** API, e.g. from Task 1.

**vTaskDelay()** API allows a Task to indicate to the RTOS that it wishes to be blocked for a specific amount of time. 
This enables the RTOS to schedule another task during this time-period.

Please see the sample code.

## Configuration of TWDT during the execution of 3 Tasks
This is a sample code for the Creation and Concurrent Execution of 3 Tasks on the ESP32 MCU by using FreeRTOS's port for ESP32, in which TWDT is also configured.

Please see the sample code.

In this code, I use the API **esp_task_wdt_init(timeout, panic)**.

Then, TWDT's default timeout value is increased to 12 seconds.

Also, toggling the "panic" argument deactivates the execution of panic handler which causes system reset.

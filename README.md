# Python_Autoclicker
This is a Python script for creating a simple auto-clicker using the pynput library. This auto-clicker listens for specific keyboard events to start and stop clicking with the mouse.

Here's an overview of how the code works:

It imports the necessary libraries: time, threading for managing threads, and pynput for mouse and keyboard input.

The code sets up some variables such as the click delay (delay), the mouse button to use (button), and the keyboard keys to start and stop the auto-clicker (start_stop_key and stop_key).

It defines a class ClickMouse that subclasses threading.Thread. This class is responsible for controlling the auto-clicking behavior. It includes methods to start and stop clicking and to exit the program.

An instance of the mouse controller (mouse = Controller()) is created, and an instance of the ClickMouse class (click_thread) is initialized with the specified delay and button.

The on_press function is defined to handle key presses. It checks if the start/stop key is pressed to toggle the auto-clicking or if the stop key is pressed to exit the program.

The Listener object is created using the on_press function as the event handler, and then it is started with listener.join() to listen for key presses.

start/stop key is  's', and the exit key is   'e'. You can adjust these keys to your preference.

The mouse button used for clicking is  the left mouse button. You can adjust it to 'Button.right' or any other mouse button according to your needs.

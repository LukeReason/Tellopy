# Luke Reason
tellopy drone flight
from djitellopy import Tello

import time

tello = Tello()

tello.connect()
tello.takeoff()
tello.get_video_capture()

# Steps 1-3
tello.move_up(102)
tello.move_forward(152)
tello.rotate_counter_clockwise(90)

# Steps 4-5
tello.move_forward(183)
tello.rotate_clockwise(90)

# Steps 6-7
tello.move_down(92)
tello.move_forward(92)
tello.rotate_clockwise(90)

# Steps 8-9
tello.move_up(31)
tello.move_forward(92)
tello.rotate_counter_clockwise(90)

# Steps 10-11
tello.move_up(61)
tello.move_forward(183)

tello.land()
tello.stop_video_capture()

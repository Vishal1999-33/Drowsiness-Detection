# About

This can be used by riders who tend to drive for a longer period of time that may lead to accidents. This code can detect your eyes and alert when the user is drowsy. There's a minimum amount of time for which one can keep his/her eyes shut. If that time is exceeded an alert will start.

# Algorithm

Each eye is represented by 6 (x, y)-coordinates, starting at the left-corner of the eye (as if you were looking at the person), and then working clockwise around the eye:

![blink_detection_plot](https://user-images.githubusercontent.com/54469035/74925313-f922f000-53f9-11ea-94e7-2c335eabdc10.jpg)

Above image shows a visualization of eye landmarks when then the eye is open.

![blink_detection_plot](https://user-images.githubusercontent.com/54469035/74925337-0b9d2980-53fa-11ea-9d38-3a58253000b4.jpg)

Above image shows eye landmarks when the eye is closed.

# Condition

It checks 40 consecutive frames and if the Eye Aspect ratio is lesst than 0.25, Alert is generated.

# Relationship

To find the Eye Aspect Ratio(EAR), we have a relationship between EAR and the 6 coordinates mentioned above. It is given be:-

![blink_detection_equation](https://user-images.githubusercontent.com/54469035/74925780-d8a76580-53fa-11ea-93b0-92f1a8dc2053.png)

Below image shows a plot between Eye Aspect Ratio and Time:-

![blink_detection_plot-1](https://user-images.githubusercontent.com/54469035/74925487-4dc66b00-53fa-11ea-8f47-f6453f591788.jpg)



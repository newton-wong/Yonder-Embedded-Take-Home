# Methodology

Replace this template with your own. Keep it short: write what a teammate would need to run your work and trust it.

## 1. How to run it

run ~python sim/launch.py --visualize

## 2. Thought process

- First, I was reading up on ROS and the QoS stuff
- Then start up all the publisher/subscriber stuff. Look at encoder_publisher.py for reference
- Work on wheel ticks and ensure that publisher/subscriber stuff is working
- How do I get the heading? first try a circle intersecting three most recent gps coordinates, easy to get angular velocity and angular velocity. I had to parameterize the circle and set heading to the derivative of the circle at the last gps point
- found out that I was overcomplicating because center of circle would be way off at 50,1, causing heading to be way off, making it unreliable
- switched to line of best fit model of the most recent 7 gps coordinates
- added everything to odometry


## 3. Known limitations

Can't find the angular velocity unless I find the line of best fit of all the headings and find the slope of that. 
On sharp turns, it might take a bit for the odometry to correctly identify the robot. 
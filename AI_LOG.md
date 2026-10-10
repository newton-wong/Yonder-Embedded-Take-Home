# AI Usage Log

Replace this template with your own entries. Add one entry per significant use of an AI tool.

## 1. <short title of what you used it for>

**What I asked:**
How to paramterize an arbitrary circle in python where t is the arc length in a cartesian coordinate grid
**What I kept vs. rewrote, and why:**
Ended up deleting most of it because this was not the soltion that I ended up with. 
**What the AI got wrong that I had to catch:**
it was pretty much correct
**How I verified it ran correctly (not just that it compiled):**
I did the paramterization math in a notebook and verified that it was correct, and then translated that math to numpy
## 2. <next use>

**What I asked:**
How to tell the direction of an arctangent of a line given the starting point (can go left to right)
**What I kept vs. rewrote, and why:**
I kept the part where they used the dot product of the vector difference of the most and least recent gps coords in consideration and used the sign of that to compute whether if I should negate the heading angle. 
**What the AI got wrong that I had to catch:**
They mixed up the negative sign for the dot product
**How I verified it ran correctly (not just that it compiled):**
I printed out all of the heading angles and verified that it was following the curve of the ground truth. 
# ENGG6400-Soft-Computing-Homework
Spring-2021 ENGG6400 HW Solution

## What I have learned from this course:
## 1. How to set the actual printed length of x, y axis to be the same in matplotlib.pyplot
I found that axes.axis('equal') will cause the x, y axis does not intersect at (0,0).
The working solution is:

```python3
axes = f.add_subplot(row, col, position)
axes.set_aspect(1.0/axes.get_data_ratio(), adjustable='box')
```


# KNN Algorithm

k-nearest neighbors (KNN) algorithm

---

## Question

|Brightness | Saturation | Color |
|-----------|------------|-------|
| 40 | 20 | red |
| 50 | 50 | blue |
| 60 | 90 | blue |
| 10 | 25 | red |
| 70 | 70 | blue |
| 60 | 10 | red |
| 25 | 80 | blue |
| 20 | 35 | ? |

---

### Solution

Lets take **K = 3**

Now calculating the distance between 20, 35 with other points and take 3 (k) data as nearest values using Euclidean distance formula:

$$\sqrt{((x_2 - x_1)^2 ) + ((y_2 - y_1)^2)}$$

| Brightness | Saturation | Color | Distance | Closest Values |
|-----------|------------|-------|----------|---|
| 40 | 20 | red | 25 | (2) |
| 50 | 50 | blue | 33.54 | (3) |
| 60 | 90 | blue | 68.00 | |
| 10 | 25 | red | 14.14 | (1) |
| 70 | 70 | blue | 61.03 | |
| 60 | 10 | red | 47.16 | |
| 25 | 80 | blue | 45.25 | |

the majority of the closest values are from red so

|Brightness | Saturation | Color |
|-----------|------------|-------|
| 20 | 35 | Red|

---

## Final table

|Brightness | Saturation | Color |
|-----------|------------|-------|
| 40 | 20 | red |
| 50 | 50 | blue |
| 60 | 90 | blue |
| 10 | 25 | red |
| 70 | 70 | blue |
| 60 | 10 | red |
| 25 | 80 | blue |
| 20 | 35 | Red |

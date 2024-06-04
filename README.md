# Problem 1: Who is in the third place?

names = ['Andi', 'Budi', 'Charlie', 'Dilan', 'Echa', 'Fanya']  
scores = [80, 90, 90, 100, 100, 80]

## Menggabungkan dua list menggunakan zip
data = list(zip(names, scores))

## Contoh cara mengakses nilai 
```python
for name, score in data:  
    print(f"{name} memiliki skor {score}")
df_dict = {}  
for i in range(len(names)):  
df_dict[names[i]] = scores[i]  
df_dict
def third_place(names, scores):  
    unique_scores = list(set(scores))  
    unique_scores.sort(reverse=True)  
third_place_names = []
    for i in range(len(scores)):  
        if scores[i] == unique_scores[2]:  
            third_place_names.append(names[i])  
print(list(range(len(scores))))  
print(third_place_names)  
    if len(third_place_names) == 1:  
print(f"The third winner: {third_place_names[0]}")  
    else:  
        names_string = ", ".join(third_place_names)  
        print(f"The third winners: {names_string}")  
third_place(names, scores)
```

# Problem 2: Find the Square Root
```python
def square_root(a, b, c):
    C = sqrt( a**2 + b**2)
    a = x(b) - x(a)
    b = y(b) - y(a)

    C = sqrt((x(b) - x(a))**2 + (y(b) - y(a))**2)
import math

def square_root(a, b, c):
    # Menghitung akar persamaan kuadrat (ax** +bx+c=0)
    discriminant = b**2 - 4*a*c
```

``` Python
 ## Memeriksa apakah terdapat solusi
    if discriminant > 0:

 # menghitung nilai X1 dan X2 ketika persamaan kuadrat memiliki dua solusi yang berbeda.
        x1 = (-b + math.sqrt(discriminant)) / (2*a)
        x2 = (-b - math.sqrt(discriminant)) / (2*a)
        return f'X1 = {x1}, X2 = {x2}'
    elif discriminant == 0:

 # berarti menentukan nilai X ketika persamaan kuadrat memiliki satu solusi.
        x = -b / (2*a)
        return f'X = {x}'
    else:
return 'No solution'

print(square_root(1, -5, 6))
print(square_root(2, 4, 2))
print(square_root(1, 1, 9))
```

# Problem 3: Find Distance Between Two Coordinates - Easy 
# d(p,q) = ((q1-p1)**2 + (q2-p2) ** 0.5) adalah rumus jarak euclidean

``` python
def distance(point_1, point_2):
    d = ((point_2[0] - point_1[0]) ** 2 + (point_2[1] - point_1[1]) ** 2) ** 0.5
    return f'The distance is {d}.'

point_1 = [5, 5]
point_2 = [1, 2]
distance (point_1, point_2)

point_1 = [0, -1]
point_2 = [-3, 2]
distance (point_1, point_2)

point_1 = [0, 7]
point_2 = [-2, 8]
distance (point_1, point_2)
```




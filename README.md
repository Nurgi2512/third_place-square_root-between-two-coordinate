# Problem 1: Who is in the third place?

names = ['Andi', 'Budi', 'Charlie', 'Dilan', 'Echa', 'Fanya']  
scores = [80, 90, 90, 100, 100, 80]

## Menggabungkan dua list menggunakan zip
data = list(zip(names, scores))

## Contoh cara mengakses nilai 
```for name, score in data:  
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

# LIST (RO'YXAT)
 
List yordamida bir o'zgaruvchida ko'p qiymatlar saqlashimiz mumkin

## LIST BILAN TANISHAMIZ

***List*** (ro'yxat) deb ataladi. Ro'yxat o'z nomi bilan, bitta o'zgaruvchida bir nechta qiymatlarni saqlash imkonini beradi. Bu qiymatlar List elementlari deyiladi. Ro'yxatda son, matn yoki aralash turdagi elementlarni saqlash mumkin. 

***List*** quyidagicha yaratiladi:

```py
this_list = ['apple', 'banana', 'charry'] # mevalar ro'yxati (matnlar)

prices_list = [12000, 26000, 40000] # narhlar ro'yxati (sonlar)

this_null_list = [] # bo'sh ro'yxat
```

Ro'yxat saqlaydigan o'zgaruvchilarni nomlashda `-lar`  (ko'plik) qo'shimchasini qo'shish maqsadga muvofiq bo'ladi (inlgiz tilida -s). 
Misol uchun: `mevalar`, `uylar`, `cars`, `toys`, `books` 

## List Elementilari

Dasturlash olamida indeks 0 dan boshlanadi! Ya'ni Listning birinchi elementing tartib raqami (indeksi) 0 ga, ikkinchi elementning indeksi 1 ga teng 

```py
mevalar = ['olma', 'anjir', 'shaftoli', "o'rik"] # mevalar ro'yxati (matnlar)
print("Birinchi meva: ", mevalar[0])
print("Ikkinchi meva: ", mevalar[1])
```

Result: `Birinchi meva: olma`

Result: `Ikkinchi meva: anjir`

Agar list ichidagi elementlar matn ko'rinishid bo'lsa, ularga [string metodlarni]() qo'llashimiz mumkin:
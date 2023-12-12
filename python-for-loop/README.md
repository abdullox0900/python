# Python For Loops

## For

Dasturlash davomida kodimizning biror qismini bir necha marta takrorlash talab etilishi mumkin. Misol uchun, ro'yxat ichidagi har bir elementni alohida qatordan konsolga chiqarish, yoki bo'lmasa har bir elementni kvdartaga oshirish va hokazo. 

Mana shunday vaziyatlarda bizga for operatori yordam beradi. Dasturlashda bu tsikl (loop) deb ataladi. 

Keling quyidagi misolni ko'ramiz. Bizda mehmonlar ro'yxati bor, biz har bir mehmonning ismini yangi qatordan chiqarmoqchimiz. Buning uchun quyidagi kodni yozamiz:

```py
mehmonlar = ['Ali','Vali','Hasan', 'Husan','Olim']

for mehmon in mehmonlar:
    print('Assalomu alaykum ' + mehmon)
```

Result: `Assalomu alaykum Ali`
Result: `Assalomu alaykum Vali`
Result: `Assalomu alaykum Hasan`
Result: `Assalomu alaykum Husan`
Result: `Assalomu alaykum Olim`

Biz ro‘yxat ichidagi har bir elementni olmoqchi bo‘lsa `for` dan foydalanamiz.

`For` so'zi ingliz tilidan `uchun` deb tarjima qilinadi.

## Looping Through a String

Faqat ro‘yxatni emas, baliq stringlarni ham biz for bilan aylana olamiz,
```py
name = 'Abdulloh'

for i = name:
    print(i)
```

Result: `A` `b` `d` `u` `l` `l` `o` `h`

har bir siringni ichidagi mantilarni birma-bir olib beradi.

Kelinglar `For`ga yana bir misol ko'raylik.

```py
mehmonlar = ['Abdulloh','Abdulbory','Jovohir', 'Bek']

for mehmon in mehmonlar: 
    print(f'Hurmatli {mehmon} sizni 20 Dekabr kuni nahorgi oshga taklif qilamiz')
    print("Hurmat bilan, Palonchiyevlar oilasi")
```

Result: `Hurmatli Abdulloh sizni 20 Dekabr kuni nahorgi oshga taklif qilamiz`
Result: `Hurmat bilan, Palonchiyevlar oilasi`

Result: `Hurmatli Abdulbory sizni 20 Dekabr kuni nahorgi oshga taklif qilamiz`
Result: `Hurmat bilan, Palonchiyevlar oilasi`

Result: `Hurmatli Javohir sizni 20 Dekabr kuni nahorgi oshga taklif qilamiz`
Result: `Hurmat bilan, Palonchiyevlar oilasi`

Result: `Hurmatli Bek sizni 20 Dekabr kuni nahorgi oshga taklif qilamiz`
Result: `Hurmat bilan, Palonchiyevlar oilasi`

## The break Statement

`break` statementi orqali ma’lum bir shartda loopni to‘xtatishimiz mumkin bo‘ladi 

Misol: 

```py
fruits = ['Apple', 'Banana', 'Cherry']

for fruit in fruits:
    print(fruit)
    if fruit == 'Banana':
      break
```

Result: `Apple` `Banana`

bu kodimiz qanday ishladi, demak biz shat berdik agar fruit == banana teng bolsa break berildi agar shart togri bolsa demo loopimiz ishlashdan toxdedi ro‘yxatining oxirigacha aylanib yurmaydi. breakdan kegin kodimiz ishlashadan to‘xtaydi.







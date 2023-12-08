# Python Challenge Day-2

## Python String Methods

Pythonda string ustida amalga oshirish mumkin bo'lgan tayyor amallar to'plami mavjud. Bunday amallar to'plami metodlar deb ataladi. 

Metodlarni qo'llash uchun metod nomi matndan so'ng `.metod_nomi()` ko'rinishida yoziladi. Keling shunday metodlarning ba'zilari bilan tanishaylik.

## (1) upper(), lower(), title(), capitalize(), strip(), lstrip(), rstrip(), replace() metodlari

1. `upper()` metodi matndagi har bir harfni katta harfga o'zgartiradi. 

```py
name = 'Abdulloh'

print(name.upper())
```

Result: `ABDULLOH`

2. `lower()` metodi har bir harfni kichik harfga o'zgartiradi.

```py
name = 'ABDULLOH'

print(name.lower())
```

Result: `abdulloh`

3. `title()` metodi matndagi har bir so'zning birinchi harfini katta harf bilan yozadi.

```py
my_job = "i'm web developer"

print(my_job.title())
```

Result: `I'm Web Developer`
 
4. `capitalize()` metodi faqatgina eng birinchi so'zning birinchi harfini katta bilan yozadi.

```py
my_job = "i'm web developer"

print(my_job.capitalize())
```

Result: `I'm web developer`

5. `strip()` metodi matndi bo'sh joylarni olib tashlaydi. (matn boshi va oxiridagi bo'shliqlarni olib tashlaydi)

```py
hi = '    Hello    '

print(hi.strip())
```

Result: `Hello`

6. `lstrip()` metodi matn boshidagi bo'shliqni olib tashlaydi.


```py
hi = '    Hello    '

print(hi.lstrip())
```

Result: `Hello    `

7. `rstrip()` metodi matn oxiridagi bo'shliqni olib tashlaydi.

```py
hi = '    Hello    '

print(hi.rstrip())
```

Result: `    Hello`

- `lstrip()` — matn boshidagi bo'shliqni,
- `rstrip()` – matn oxiridagi bo'shliqni,
- `strip()` — matn boshi va oxiridagi bo'shliqlarni olib tashlaydi

```py
meva = "     olma     "

print("Men " + meva.lstrip() + " yaxshi ko'raman")
print("Men " + meva.rstrip() + " yaxshi ko'raman")
print("Men " + meva.strip() + " yaxshi ko'raman")
print("Men " + meva + " yaxshi ko'raman")
```

```txt
Men olma      yaxshi ko'raman 
Men       olma yaxshi ko'raman 
Men olma yaxshi ko'raman 
Men       olma      yaxshi ko'raman
```

### ❗️ Metodlar o'zgaruvchi ichidagi asl matnni o'zgartirmaydi!

Matnlar bilan ishlaydigan metodlar ko'p. to'liq ro'yhatni esa quyidagi [sahifada](https://www.w3schools.com/python/python_ref_string.asp) ko'rishingiz mumkin.

8. `replace()` orqali bir matn ichidagi so‘zni o‘zgartirishimiz mumkin boshqa so‘zga.

```py
txt = 'Hello World'

print(txt.replace('Hello', 'Salom'))
```

Result: `Salom World`

❗️bu barcha shunday matnlarni o‘zgartiradi.

```py
txt = 'Hello World, Hello Alisher, Hello Bek'

new_txt = txt.replace('Hello', 'Salom')

print(new_txt)
```

Result: `Salom World, Salom Alisher, Salom Bek`


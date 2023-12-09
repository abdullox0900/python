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

## (2) startswich(), endswich(), find(), index(), split(), join()

1. `startswich()` bu metod o'zgaruvchi ichida biz xohlagan matn bormi yakmi tekshirib beradi. (o'zgaruvchini boshidan)

```py
txt = 'Hello World'

new_txt = txt.startswich('Hello')

print(new_txt)
```

Result: `True`


2. `endswich()` bu metod 'zgaruvchi ichida biz xohlagan matn bormi yakmi tekshirib beradi fakat oxiridan. (o'zgaruvchini oxiridan)

```py
txt = 'Hello World'

new_txt = txt.endswich('World')

print(new_txt)
```

Result: `True`

3. `index()` and `find` bu metodlar matning bosh harfi nechanchi indeksda turganini qaytaradi.

- `index()`

```py
txt = 'Hello World, Apple'

new_txt = txt.index('World')
new_txt_2 = txt.index('Apple')

print(new_txt)
print(new_txt_2)
```

Result: `6`

Result: `13`

- `find()`

```py
txt = 'Hello World Apple'

new_txt = txt.find('World')
new_txt_2 = txt.find('Apple')

print(new_txt)
print(new_txt_2)
```

Result: `6`
Result: `13`

❗️ `index()` va `find()` bir xil vazifani bajaradi, lekin ularning ma’lum bir farqi bor.

`index()` biz bergan mantini topa olmasa bizga javoban error qaytaradi. 
`find()` esa bizga javoban `-1` qaytaradi

```py
txt = 'Hello World'

new_txt_index = txt.find('Apple')
new_txt_find = txt.find('Apple')

print(new_txt_index)
print(new_txt_find)
```

Result index: `ValueError: substring not found`

Result fint: `-1`

4. `spit()` bu metod oddiy matini listga ogirib beradi

```py
txt = 'apple orangem kiwi banana'

new_txt_list = txt.split()

print(new_txt_list)
```

Result: `['apple', 'orange', 'kiwi', 'banana']`

5. `join()` metod listni matnga ogirib beradi

```py
x_list = ['apple', 'orange', 'kiwi', 'banana']

txt = ' '.join(x_list)

print(txt)
```

Result: `apple orange kiwi banana`


## All python strint methods lenght: 43

### 1. Conversion:

- `str.capitalize()`
- `str.lower()`
- `str.upper()`
- `str.title()`
- `str.swapcase()`

### 2. Information:

- `str.count(substring)`
- `str.endswith(suffix)`
- `str.startswith(prefix)`
- `str.find(substring) or str.index(substring)`
- `str.isalnum()`
- `str.isalpha()`
- `str.isnumeric()`
- `str.islower()`
- `str.isupper()`

### 3. Modification:

- `str.replace(old, new)`
- `str.strip([chars])`
- `str.lstrip([chars])`
- `str.rstrip([chars])`
- `str.join(iterable)`
- `str.partition(separator)`
- `str.rpartition(separator)`
- `str.center(width[, fillchar])`
- `str.ljust(width[, fillchar])`
- `str.rjust(width[, fillchar])`
- `str.zfill(width)`

### 4. Testing:

- `str.isalnum()`
- `str.isalpha()`
- `str.isdigit()`
- `str.isspace()`
- `str.isdecimal()`
- `str.isidentifier()`
- `str.isprintable()`

### 5. Splitting and Joining:

- `str.split([sep[, maxsplit]])`
- `str.rsplit([sep[, maxsplit]])`
- `str.splitlines([keepends])`
- `str.join(iterable)`

### 6. Formatting:

- `str.format()`
- `str.format_map(mapping)`
- `str.lstrip([chars])`
- `str.rstrip([chars])`
- `str.strip([chars])`

### 7. Encoding and Decoding:

- `str.encode([encoding[, errors]])`
- `str.decode([encoding[, errors]])`
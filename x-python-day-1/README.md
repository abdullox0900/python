# Python Challenge Day-1

### VARIABLE (O'ZGARUVCHI)

O'zgaruvchi — kompyuter xotirasida ma'lum bir qiymatni saqlash uchun ajratilgan joy. Soddaroq qilib tushuntirsak, o'zgaruvchini quti, quti ichidagi narsani esa qiymat deb tasavvur qilish mumkin. Pythonda qiymatlar son, matn, ro'yxat va hokazo ko'rinishida bo'lishi mumkin.

1. Pythonda o'zgaruvchi yaratish

```py
ism = 'Abdulloh'
yosh = 20

print(ism)   # Abdulloh
print(yosh)  # 20
```

O'zgaruvchi (variable) bunday deyilishiga sabab, uning qiymati istalgan vaqt o'zgartirilishi mumkin:

```py
ism = "Abdulloh"
print(ism)  # Abdulloh
ism="Muhammad"
print(ism)  # Muhammad
```

2. O'zgaruvchi nomlash

- O'zgaruvchilarga nom berishda quyidagi qoidalarga amal qiling:
- O'zgaruvchi nomi harf yoki pastki chiziq (_) bilan boshlanishi kerak
- O'zgaruvchi nomi raqam bilan boshlanishi mumkin emas
- O'zgaruvchi nomida faqatgina lotin alifbosi harflari (A-z), raqamlar (0-9) va pastki chiziq (_) qatnashishi mumkin
- O'zgaruvchi nomida bo'shliq (пробел) bo'lishi mumkin emas
- O'zgaruvchi nomida katta-kichik harflar turlicha talqin qilinadi (ism, ISM, va Ism uchta turli o'zgaruvchi)

3. Qo'shimcha qoida sifatida: 

- O'zgaruvchi nomini kichik harflar bilan yozing. 
- O'zgaruvchi nomida 2 va undan ortiq so'z qatnashsa ularning orasini pastki chiziq `(_)` bilan ajrating `(ism_sharif="Anvar Narzullaev")`
- O'zgaruvchiga tushunarli nom bering `(y=20 emas yosh=20, d="Korea" emas davlat = "Korea" va hokazo)`
- Shuningdek o'zgaruvchilarga Pythonda ishlatiladigan funktsiyalar va maxsus kalit so'zlarning `(keywords)` nomini bermang. Kalit so'zlar ro'yhatini ko'rish uchun konsolda `help()` deb yozing va Enter tugmasini bosing. Keyin esa `(keywords)` deb kiritib, yana Enter bosing. Marhamat, ekraningizda Pythondagi maxsus kalit so'zlar ro'yhatini ko'ryapsiz:

4. Python keywords

```py
False               class               from                or
None                continue            global              pass
True                def                 if                  raise
and                 del                 import              return
as                  elif                in                  try
assert              else                is                  while
async               except              lambda              with
await               finally             nonlocal            yield
break               for                 not                 
```

### STRING (MATN)

1. String

STRING (matn) —Pythondagi eng mashxur ma'lumot turlaridan biri. o'zgaruvchiga matn yuklash uchun matn qo'shtirnoq `(" ")` yoki birtirnoq `(' ')`ichida yozilishi kerak.

```py
country = 'Uzbekistan'
city = "Andijon"
```

Pythonda matnlar [Unicode](https://symbl.cc/en/unicode/table/) jadvalidagi istalgan belgilaridan iborat bo'lishi mumkin (jumladan o'zbek, arab, hind, xitoy alifbosidagi harflar yoki turli emoji-smayliklar). 

```py
new_str = "I'm emoji 🙂"
print(new_str)
```

Result: `I'm emoji 🙂`


### Matnlarni qo'shish operatori (+)

Matnlarni qo'shish uchun `+` operatoridan foydalanmiz:

```py
name = 'Abdulloh'

print('My name is ' + name)
```

Result: `My name is Abdulloh`

```py
first_name = 'Abdulloh'
last_name = 'Abdusalomov'

print(first_name + last_name)
```

Result: `AbdullohAbdusalomov`

Yuqoridagi kodda ism va familiya orasiga bo'shliq belgisini qo'shmaganimiz uchun ikki matn qo'shilib yozildi. Buni to'g'rilash uchun, 3-qatorni quyidagicha yozamiz:

```py
first_name = 'Abdulloh'
last_name = 'Abdusalomov'

print(first_name + ' ' + last_name)
```

Result: `Abdulloh Abdusalomov`

### f-string

Ikki (va undan ko'p) matn ko'rinishidagi o'zgaruvchilarni birlashtirish uchun f-string usulidan  `f"{matn1} {matn2}"` ham foydalansak bo'ladi:

Bu usul yordamida uzun matnlarni ham yasash mumkin:

```py
first_name = 'Abdulloh'
my_job = 'Web Developer'
result = f"Hi, My name is {first_name} I'm {my_job}"

print(result)
```

Result: `Hi, My name is Abdulloh I'm Web Developer`

### Mahsus belgilar

Matnga bo'shliq qo'shish uchun `\t` belgisidan, yangi qatordan boshlash uchun `\n`belgisidan foydalanamiz:

```py
print('Hello World!')
print('Hello \t World!')
print('Hello \n World!')
```

Result:

`Hello World!`

`Hello     World!`

`Hello`

`World!`

### Basic Operations
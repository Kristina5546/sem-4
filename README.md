# sem-4

#Задача 1
#Вычислить число c заданной точностью d

#Пример:

#- при $d = 0.001, π = 3.141.$    $10^{-1} ≤ d ≤10^{-10}$

#import math

#d = input('Введите степень округления в формате 0.01 от 10 в степени -1 до 10 в степени -10 -> ')
#d = d[2:len(d)]
#print (round(math.pi, len(d)))


#Задача 2.
#Задайте натуральное число N. Напишите программу, которая составит список простых множителей числа N.

#n = int(input('Введите число -> '))
#spisok = [n]


#def prosto(spisok):
#    fl = 0
#    for i in range(spisok[-1] // 2, 1, -1):
#        if spisok[len(spisok) - 1] % i == 0:
#            spisok.append(i)
#            spisok[-2] = spisok[-2] // i
#
#    if fl != 0:
#        prosto(spisok)


#prosto(spisok)

#print(spisok)

#Задача 3.
Задайте последовательность чисел. Напишите программу, которая выведет список неповторяющихся элементов исходной последовательности.

#a = [5, 3, 4, 9, 5, 6, 7, 8, 9, 5, 3]
#b = set(a)
#print(b)

#Задача 4.
#Задана натуральная степень k. Сформировать случайным образом список коэффициентов (значения от 0 до 100) многочлена и записать в файл многочлен степени k.

#Пример:

#- k=2 => 2*x² + 4*x + 5 = 0 или x² + 5 = 0 или 10*x² = 0

#from random import randint


#k = int(input('Введите число -> '))
#a = randint(0,100)
#b = randint(0,100)
#c = randint(0,100)
#with open('C:\Users\Кристина\OneDrive\Рабочий стол\PY\app.py.txt', 'w', encoding='utf-8') as file:
#   file.write(f'{a}*x^{k} + {b}*x + {c} = 0')


#Задача 5.
#Даны два файла, в каждом из которых находится запись многочлена. Задача - сформировать файл, содержащий сумму многочленов.


with open('C:\Users\Кристина\OneDrive\Рабочий стол\PY\app.py.txt', 'r') as file:
   mnog1 = file.read()
   mnog1 = mnog1[0:-4]

with open('C:\Users\Кристина\OneDrive\Рабочий стол\PY\app.py.txt', 'r') as file:
   mnog2 = file.read()

with open('C:\Users\Кристина\OneDrive\Рабочий стол\PY\app.py.txt', 'w', encoding='utf-8') as file:
   file.write(f'{mnog1} + {mnog2}')

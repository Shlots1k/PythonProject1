import random

a = float(input("Введіть число a: "))
b = float(input("Введіть число b: "))

operation = input("Введіть дію (+, -, *, /): ")

if operation == "+":
    print("Результат:", a + b)

elif operation == "-":
    print("Результат:", a - b)

elif operation == "*":
    print("Результат:", a * b)

elif operation == "/":
    if b == 0:
        print("Ділення на нуль")
    else:
        print("Результат:", a / b)

else:
    print("Невідома операція")



points = int(input("Введіть кількість балів: "))

if 0 <= points <= 49:
    print("Незадовільно")
elif 50 <= points <= 69:
    print("Задовільно")
elif 70 <= points <= 89:
    print("Добре")
elif 90 <= points <= 100:
    print("Відмінно")
else:
    print("Неможлива кількість балів")



fak = int(input("Введіть число : "))

factorial = 1
for i in range(1, fak + 1):
    factorial *= i

print("Факторіал ", fak, ":", factorial)



num11 = int(input("Введіть число : "))

for i in range(num11, 0, -1):
    if i % 2 == 0:
        print(i, end=" ")


num1 = int(input('\nВведіть перше число - '))
num2 = int(input('Введіть друге число - '))
for i in range(num1, num2 + 1):
    print(i)


number = random.randint(1,10)
num1 = 0
life = 0
while num1 != number:
    life += 1
    num1 = int(input('Вгадайте число в діапазоні цих чисел - '))
    if num1 == number:
        print('Ви вгадали число!')
        print(('Кількість спроб - '),life)
        break
    elif life == 4:
        print('YOU LOSE')
    if num1 >= number:
        print('Це число менше за це')
    else:
        print('Це число більше за це')


print('Ви вгадали число!')


age = int(input("Enter your age: "))
name = input("Enter your name: ")
print('Привіт',name,'тобі',age)

age1 = int(input("Enter your age: "))
if age1 > 18:
    print('Welcome')
else:
    print('Sorry, you are not 18 years old')

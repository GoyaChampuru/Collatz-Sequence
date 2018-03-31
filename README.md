# Collatz-Sequence
Practice Project for ATBS CH.4

def collatz(number):
    if number % 2 == 0:
        return number // 2
    elif number % 2 == 1:
        return 3 * number + 1


try:
    number = int(input('Enter an integer greater than 1: '))
    print(number)
    while number != 1:
        number = collatz(number)
        print(number)
except ValueError:
    print('Error: Please enter a valid number.')

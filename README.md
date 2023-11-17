# init.py:

from operations import add, subtract, multiply, divide, power, modulus

def game():
    score = 0
    while True:
        print('======== Menu ========'
              '\n1. Add'
              '\n2. Subtract'
              '\n3. Multiply'
              '\n4. Divide'
              '\n5. Power'
              '\n6. Modulus'
              '\n0. Exit')
        option = int(input('\nChoose an option: '))
        if option == 0:
            break
        num_1 = int(input('Enter first number: '))
        num_2 = int(input('Enter second number: '))
        answer = int(input('Enter your answer: '))

        if option == 1:
            result = add(num_1, num_2)
        elif option == 2:
            result = subtract(num_1, num_2)
        elif option == 3:
            result = multiply(num_1, num_2)
        elif option == 4:
            result = divide(num_1, num_2)
        elif option == 5:
            result = power(num_1, num_2)
        elif option == 6:
            result = modulus(num_1, num_2)

        if result == answer:
            if option in [1, 2]:
                score += 1
            elif option in [3, 4]:
                score += 2
            elif option in [5, 6]:
                score += 4
            print('Correct!!')
        else:
            print('Incorrect')

    print(f'======== Game Over ========'
          f'\nYour score is {score}'
          '\nKeep going!')

if __name__ == "__main__":
    game()


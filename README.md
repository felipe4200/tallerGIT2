# operations.py:
def add(num_1, num_2):
    result = num_1 + num_2
    print(f'{num_1} + {num_2} is equal to {result}')
    return result

def subtract(num_1, num_2):
    result = num_1 - num_2
    print(f'{num_1} - {num_2} is equal to {result}')
    return result

def multiply(num_1, num_2):
    result = num_1 * num_2
    print(f'{num_1} * {num_2} is equal to {result}')
    return result

def divide(num_1, num_2):
    if num_2 != 0:
        result = num_1 / num_2
        print(f'{num_1} / {num_2} is equal to {result}')
        return result
    else:
        print('Cannot divide by zero!')
        return None

def power(num_1, num_2):
    result = num_1 ** num_2
    print(f'{num_1} ^ {num_2} is equal to {result}')
    return result

def modulus(num_1, num_2):
    if num_2 != 0:
        result = num_1 % num_2
        print(f'{num_1} % {num_2} is equal to {result}')
        return result
    else:
        print('Cannot calculate modulus with zero!')
        return None

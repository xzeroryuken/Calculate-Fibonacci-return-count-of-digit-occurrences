def fib(n):
    myList = []
    
    x = 0
    y = 1
    myList.append(x)
    myList.append(y)
    for i in range(2, n + 1):
        y = x + y
        x = y - x
        myList.append(y)
    
    counts = count_digits(myList)
    
    result = [(count, digit) for digit, count in counts.items()]
    result.sort(reverse=True)
    return result
    
def count_digits(myList):
    counts = {}
    for digit in str(myList[-1]):
        if digit.isdigit():
            if digit not in counts:
                counts[digit] = 1
            else:
                counts[digit] += 1
    return counts

print(fib(10000))

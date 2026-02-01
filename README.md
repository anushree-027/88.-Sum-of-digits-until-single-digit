# 88.-Sum-of-digits-until-single-digit
number = int(input("Enter number: "))
step = 1

while number > 9:
    total_sum = 0
    temp = number
    while temp:
        total_sum += temp % 10
        temp //= 10
    print(f"Step-{step} Sum: {total_sum}")
    number = total_sum
    step += 1

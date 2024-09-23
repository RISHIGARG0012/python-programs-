start = int(input("Enter the starting point: "))
end = int(input("Enter the ending point: "))
orien = input("Enter 'horizontal' or 'vertical': ")
order = input("Enter 'forward' or 'reverse': ")
if order == 'forward':
    if orien == 'horizontal':
        print(" ".join(str(i) for i in range(start, end + 1)))
    elif orien == 'vertical':
        for i in range(start, end + 1):
            print(i)
    else:
        print("Invalid orientation choice. Please enter 'horizontal' or 'vertical'.")

elif order == 'reverse':
    if orien == 'horizontal':
        print(" ".join(str(i) for i in range(end, start - 1, -1)))
    elif orien == 'vertical':
        for i in range(end, start - 1, -1):
            print(i)
    else:
        print("Invalid orientation choice. Please enter 'horizontal' or 'vertical'.")

else:
    print("Invalid order choice. Please enter 'forward' or 'reverse'.")

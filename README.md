# Experiment-5
## AIM:
Write a python program for Binary Search and inspect for failures. 

# ALGORITHM

1. Start the program.

2. Get the list from the user

3. Get the element to be searched

4. Compare the mid element with the key, if same return the index

5. If key is greater, search it in the right side, else search it in the left side.

6. If not found return -1

7. Stop the program. 

 # PROGRAM
~~~
def binary_search(arr, x):
    low = 0
    high = len(arr) - 1
    mid = 0

    while low <= high:
        mid = (high + low) // 2

        if arr[mid] < x:
            low = mid + 1
        elif arr[mid] > x:
            high = mid - 1
        else:
            return mid  # Fixed return value

    return -1  # Moved return -1 outside the loop


arr = [2, 3, 4, 10, 40]

try:
    x = int(input("Enter the element to be searched: "))  # Fixed quotes
    result = binary_search(arr, x)

    if result != -1:
        print("Element is present at index", str(result))
        print("Test Case:Pass")
    else:
        print("Element is not present in array")
        print("Test Case:Pass")

except ValueError:  # Catching specific exception
    print("Enter a valid input!")
    print("Test Case:Fail")

~~~
 # OUTPUT
 ![Screenshot 2025-03-27 102856](https://github.com/user-attachments/assets/ab39b00b-0a56-4a4a-af75-cf3a02c50be6)

 ![Screenshot 2025-03-27 102934](https://github.com/user-attachments/assets/77e68a29-50f0-4387-8ac9-a3d9863bd4fe)

![Screenshot 2025-03-27 103003](https://github.com/user-attachments/assets/faedb4e6-ab6a-4af8-a9a8-576613154fac)

![Screenshot 2025-03-27 103043](https://github.com/user-attachments/assets/132c198d-4b38-461d-a646-2775f76907c3)

![Screenshot 2025-03-27 103143](https://github.com/user-attachments/assets/f23afe2a-101f-44ba-b87b-2a55322f2ada)

![Screenshot 2025-03-27 103230](https://github.com/user-attachments/assets/cb34e09c-f77a-4bc8-9326-470448c59ab4)

![Screenshot 2025-03-27 103338](https://github.com/user-attachments/assets/9b057896-e3b6-42aa-a9af-1710ce2eb5f1)

![Screenshot 2025-03-27 103356](https://github.com/user-attachments/assets/7d6af16c-4363-4807-9879-fac2046a0968)


# RESULT

Thus, the python program of binary search is implemented and the output is verified
successfully. 

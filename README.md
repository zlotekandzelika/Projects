#for loops 
for i in range(5):
    print(i)
    
#while loops 
counter = 0
while counter <5:
    print(counter)
    counter+=1   

    person={
    "name":"bob", "age":"25", "city": "techland" 
}

#accessing values 
print(person["name"])

#modifing values 
person["age"]=26 

print(person)

def merge_sort(arr):
    if len(arr) > 1:
        mid = len(arr) // 2
        left_half = arr[:mid]
        right_half = arr[mid:]

        merge_sort(left_half)
        merge_sort(right_half)

        i = j = k = 0

        while i < len(left_half) and j < len(right_half):
            if left_half[i] < right_half[j]:
                arr[k] = left_half[i]
                i += 1

            else:
                arr[k] = right_half[j]
                j += 1
                k += 1 

                while i < len(left_half):
                    arr[k] = left_half[i]
                    i += 1
                    k += 1 

                    while j < len(right_half):
                        arr[k] = right_half[j]
                        j += 1
                        k += 1 

my_list = [64,25,12,22,11]
merge_sort(my_list)

def binary_search(arr, target):
    low, high = 0, len(arr) - 1 

    while low <= high:
        mid = (low + high) // 2 
        mid_element = arr[mid] 

        if mid_element == target: 
            return mid 
        elif mid_element < target: 
            low = mid + 1 
        else: 
            high = mid - 1 

            return -1 
            
my_list = [11,12,22,25,64]
target_element = 12 
result = binary_search(my_list, target_element)
print(f"Element {target_element} found at index {result}" if result != -1 else f"Element {target_element} not found")
    

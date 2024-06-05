def binary_search(arr,target):
    left, right = 0, len(arr) -1
    
    while left <= right:
        mid = (left+right)//2
        if arr[mid] == target:
            return mid
        elif arr[mid]<target:
            left = mid+1
        else:
            right = mid -1
    return -1
    
arr = [2,6,7,8,9,14,15,18]
target = 15
result = binary_search(arr,target)
if result != -1:
    print(f"element {target} found at index {result}")
else:
    print(f"element {target} not found in the array")# binary-search

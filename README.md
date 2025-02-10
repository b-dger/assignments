def sort_descending(lst):
    n = len(lst) # gets length of the list
    for i in range(n): # loop through each index of range of n in list
        max_idx= i # current index i is = to the largest value
        #find index of max element in the unsorted list
        for j in range(i+1, n): #loop through the rest of the list
                if lst[j] > lst[max_idx]: # if any value in the list is large than the current max
                    max_idx = j # update max to the index of the new largest value
        lst[i], lst[max_idx] = lst[max_idx], lst[i] # swap largest value found with the value at index i
    return lst #return sorted list

list = [2, 5, 3, 1, 4, 7, 6]
sorted_list = sort_descending(list) #call sorting function
print("sorted list(descending):", sorted_list) #print sorted list

# calculate sum of the list and divide it by thge length of list
def average(list): #define function average
    n = len(list) # n = to the length of list
avg = sum (list) / len (list) # avg = the sum of the list and divides it by the length
print("average:", avg) # prints avg of the list

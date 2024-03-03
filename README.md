# minandmaxnums
def find_max(numlist):
     maxval = float('-inf')
     for x in numlist: 
         if x > maxval:
             maxval = x
     return maxval
     
def find_min(numlist):
    minval = float('+inf')
    for y in numlist:
        if y < minval:
            minval = y
    return minval
    
numbers = input("Enter a list of numbers: ")
numlist = numbers.split()
for i in range(len(numlist)):
    numlist[i] = int(numlist[i])
    
minimum = find_min(numlist)
maximum = find_max(numlist)
print("Minimum: ", minimum)
print("Maximum: ", maximum)

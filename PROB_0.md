# Strictly Increasing
Given an array, determine if the array is strictly increasing with up to 3 exceptions.

def strictIncr(array)  
    countEx = 0  
    last = -1  
    for i in array  
        if last > i  
            countEx += 1  
        if countEx > 3  
            return false  
        last = i  
    return true  

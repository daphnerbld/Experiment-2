# EXPERIMENT 2
**NUMERICAL PYTHON (NUMPY)**
Daphne P. Robleado
*2ECE-A*
September 1, 2024
* **NORMALIZATION PROBLEM:**

Indented code

    import numpy as np
    #Making and printing a random 5x5 array matrix
    
    X = np.random.rand(5, 5)
    
    print("Original ndarray X:")
    print(X)
    
    #Normalization function
    mean = X.mean()
    std_dev = X.std()
    
    X_normalized = (X - mean) / std_dev
    print("\nNormalized ndarray:")
    print(X_normalized)
    
    #saving the value of normalization function
    np.save('X_normalized.npy', X_normalized)

* **DIVISIBLE BY 3 PROBLEM**

Indented code

    import numpy as np
    
    #Creating a matrix of perfect square values from 1-100
    A = np.array([i**2 for i in range(1, 101)])
    
    #Reshaping it to 10x10
    A = A.reshape(10, 10)
    
    #Printing the values
    print("Squared values from 1-100:")
    print(A)
    
    #Divisible by 3 function
    div_by_3 = A[A % 3 == 0]
    
    print("\nElements divisible by 3:")
    print(div_by_3)
    
    #Saving the value of the function as np
    np.save('div_by_3.npy', div_by_3)

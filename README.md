# Find_Prime_Numbers_In_A_Range
This code is to find out the prime numbers between a given range.


    def print_prime_nembers(x, y):

        c = []
    
        for i in range(x, y):
            b = []
            for a in range(1, i + 1):
                if i % a == 0:
                    b.append(a)
            c.append(b)
    
        prime_factors = []
    
        for factors in c:
            if len(factors) == 2:
                prime_factors.append(factors)
    
        for char in prime_factors:
            print(char[-1])
        
    x, y = map(int, input(f"Enter a range of digit seperated by space to print prime numbers : ").split())
    print_prime_nembers(x, y)

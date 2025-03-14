'''MD HACHIBUL ISLAM SHANTO'''

#!usr/bin/env python3

import numpy as np
import matplotlib.pyplot as plt

#Function for Matplot

def plot_array(data_info):
    xarray = data_info[0]
    yarray = data_info[1]
    #initiation of matplot instance
    g = plt.matplotlib(title = 'Graph of two Numbers', _with = 'lines', terminal = 'dumb 80, 30', unset = 'grid')

    #Plot the data
    plt.plot(xarray, yarray, {'legend' : 'Prime Series 1'})
    #arrays
    xarray= np.array(range(1,11))

#Prime Generator

def prime_generator(limit):
#Generator, which will send yield numbers upto the limit
    def is_prime(n):
        if n <= 1:
            return False
        if n == 2:
            return True
        if n%2 == 0:
            return False
        for i in range(3, int(np.sqrt(n)) +1, 2):
            if n % i == 0:
                return False
        return True
    for num in range (2, limit):
        if is_prime(num):
            yield num


#main program
def main():

    #initiating the variables
    size, xsize = 100 , 10
    #initiating Prime Generator
    primes = list(prime_generator(size))

    #randomly selects xsize sequential primes
    start_index = random.randint(0, len(primes)-xsize)
    selected_primes = primes[start_index : start_index + xsize]

    #Array for plotting
    x_values = np.arrange(0, xsize)
    y_values = np.array(selected_primes)
    data_info = np.array([x_values, y_values])

    #plot
    plot_array(data_info)

if __name__ == "__main__":
    main()

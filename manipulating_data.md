### I can manipulate data, and use different functions and methods to describe it
#### These are examples where I performed conversions, applied methods, and functions to the data.
In [0]:

    ean_rt= np.mean(rt_conversion).round(1) 
    print(“Mean RT = “ + str(mean_rt) + “ ms”)

In [0]:

    std_rt = np.std(rt_conversion).round(2) 
    print(“Standard deviation = “ + str(std_rt) + “ ms”)

#### To further manipulate data, I can create loops to serve different purposes

In [0]:

    for index in more_rt: 
        rt.append(index) for index in more_err: 
            err.append(index)

### I am able to visualize data in different ways

#### Here is an example where I used different functions to perform image analysis

    plt.imshow(ndi.rotate(vol[:, :, 79], angle = 180), cmap='gray')
    plt.axis('off')
    plt.show()


<img width="200"  src=''>

### Here is an example of using seaborn to visualize data
In [0]:

    # Error rate barplot showing simon and flanker conditions
    sns.catplot(kind = 'bar', data = df, y = 'error', hue = 'simon', x = 'flankers', palette = 'colorblind', ci=None)
    plt.title('Figure 2 (ERROR RATE)')
    plt.show()
    


#### This is how I can use subplots to further organize my data visualization

    fig = plt.figure(figsize = [8, 12])
    subplot_counter = 1

    # Loop through subplots and draw an image 
    for ii in range (0, 160, 10): 
        fig.add_subplot(4, 4, subplot_counter) 
        plt.imshow(vol[ii], cmap='gray')
        plt.axis('off')
        plt.tight_layout()
        subplot_counter += 1 
    #render the figure 
    plt.show()

#### I am also able to mask different images

<img width="200"  src='a-6.png'>

#### Finally, I can overlay colormaps

<img width="200"  src='a-7.png'>

     

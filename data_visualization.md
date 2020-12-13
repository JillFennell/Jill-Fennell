### I am able to visualize data in different ways[¶](#I-am-able-to-visualize-data-in-different-ways) {#I-am-able-to-visualize-data-in-different-ways}

#### Here is an example where I used different functions to perform image analysis

In [0]:

    plt.imshow(ndi.rotate(vol[:, :, 79], angle = 180), cmap='gray')
    plt.axis('off')
    plt.show()

### Here is an example of using seaborn to visualize data
In [0]:

    # Error rate barplot showing simon and flanker conditions
    sns.catplot(kind = 'bar', data = df, y = 'error', hue = 'simon', x = 'flankers', palette = 'colorblind', ci=None)
    plt.title('Figure 2 (ERROR RATE)')
    plt.show()
    


#### This is how I can use subplots to further organize my data visualization

In [0]:

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



#### Finally, I can overlay colormaps

In [0]:

     

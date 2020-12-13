### Here is an example of importing data:


    import imageio
    import scipy.ndimage as ndi
    import scipy.stats
    import nibabel as nib
    import numpy as np
    import matplotlib.pyplot as plt


    files = glob(‘X/_data.txt’) dataframes = [pd.read_csv(x, sep=’\t’) for x in files]

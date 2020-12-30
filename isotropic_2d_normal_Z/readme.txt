-Generated data:  
    Distribution: 2d isotropic gaussian with mean=[-2,0] and cov = [[1,0],[0,100]]
    sample size: 20000
    
-Model:
latent dim: 2
hidden dim: 128
batch_size: 32
learning rate: 1e-3
# epoch: 20

-Testing:
--with 10000 samples from prior ~ N([0,0],[[1,0],[0,1]])
--with 10000 samples from the same distribution of the training data (test encoder)
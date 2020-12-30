-Generated data:  
    See Appendix H.1 in (http://www.gatsby.ucl.ac.uk/~balaji/udl2020/accepted-papers/UDL2020-paper-056.pdf)
    sample size: 40000
    
-Model:
latent dim: 2
hidden dim: 128
batch_size: 64
learning rate: 1e-5
# of epochs: 200

Problem-- cannot converge due to initialized log(sigma) being too large => large z => large L(log(p_z))
log sigma clamp: max=10           note: exp(10)=22026.47

-Testing:
--with 20000 samples from prior ~ N([0,0],[[1,0],[0,1]])
--with 20000 samples from the same distribution of the training data (test encoder)

-The loss is still decreasing; but from the generated samples from prior becomes less alike to the original distribution. (Epoch #45 vs #70 vs #120)
-It's because the assumption of X should be gaussian?

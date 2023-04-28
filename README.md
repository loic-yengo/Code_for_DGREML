This folder contains various source code used to 
1) simulate Assortative mating (src_simAM_05Jan2022.tar.gz)
2) simulate correlated Bernoulli distributed variables, mimicking allele distribution in an assortatively mating equilibrium population (src_simCorrBin.tar.gz)

This code needs an Eigen library to be compiled. Once compiled, options can be accessed by typing ./simAM --help

Example for (1)

./simAM \
  
  
  --r 0.2 \        # spousal correlation
  
  
  --n 10000 \      # Population size
  
  
  --m 10000 \      # Number of (causal) variants
  
  
  --nchr 10 \      # Number of chromosomes
  
  
  --p 0.5 \        # Allele frequency  
  
  
  --h2eq 0.8 \     # Heritability in the equilibrium population
  
  
  --make-ped \     # Output genotypes in PLINK text format
  
  
  --ng 10 \        # Number of generation of 
  
  
  --nc 1000 \      # Size of the pool of mates each person can access
  
  
  --seed1 100101 \ # Random number geneteror seed to control sampling of effect size distribution
  
  
  --seed2 200383 \ # Random number geneteror seed to control sampling of genotypes


  --nthreads 10 \  # Number of threads used to run the simulation
  
  
  --out mySim      # Prefix for output files.

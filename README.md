# ResearchKit Bookmarks
Open source internal and extended research, We use in our internal and commercial projects.

**Focus in**
- Data Structures and Algorithms
- Machine Learning, Deep Learning and AI

# Butterworth Band Pass
Signal processing filter
- https://en.wikipedia.org/wiki/Butterworth_filter

**Python**
- https://scipy-cookbook.readthedocs.io/items/ButterworthBandpass.html

**iOS**
```
 float A = sqrt(pow(10.0f, (G/20.0f)));
 float beta = sqrt(A / Q);
 
 a0 = (A + 1) - ((A - 1) * omegaC) + (beta * omegaS);
 b0 = (A * ((A + 1) + ((A - 1) * omegaC) + (beta * omegaS)))     / a0;
 b1 = (-2 * A * ((A - 1 ) + ((A + 1) * omegaC)))                 / a0;
 b2 = (A * ((A + 1) + ((A - 1) * omegaC) - (beta * omegaS)))     / a0;
 a1 = (2 * ((A - 1) - ((A + 1) * omegaC)))                       / a0;
 a2 = ((A + 1) - ((A - 1) * omegaC) - (beta * omegaS))           / a0;
```

# ResearchKit Bookmarks
Open source internal and extended research, We use in our internal and commercial projects.

**Focus in**
- Data Structures and Algorithms
- Machine Learning, Deep Learning and AI

# Algorithms
## Butterworth Band Pass
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

## k-NN
Pattern recognition
https://en.wikipedia.org/wiki/K-nearest_neighbors_algorithm

An easy way to evaluate the accuracy of the model is to calculate a ratio of the total correct predictions out of all predictions made.

Let’s create a getAccuracy function which sums the total correct predictions and returns the accuracy as a percentage of correct classifications.

**Python**
```
def getAccuracy(testSet, predictions):
    correct = 0
    for x in range(len(testSet)):
        if testSet[x][-1] is predictions[x]:
            correct += 1
    return (correct/float(len(testSet))) * 100.0
```
```
testSet = [[1,1,1,'a'], [2,2,2,'a'], [3,3,3,'b']]
predictions = ['a', 'a', 'a']
accuracy = getAccuracy(testSet, predictions)
print(accuracy)
```



# Machine Learning and Deep Learning
- **Tensorflow** - https://github.com/tensorflow
- **PyTorch** - https://github.com/pytorch/pytorch
- **Keras** - https://keras.io/api/
- **MXNet** https://github.com/apache/incubator-mxnet

Nueral Network:
- **Chainer** - https://github.com/chainer/chainer
- **Sonne** - https://github.com/deepmind/sonnet

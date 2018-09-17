# d8
#numpy
import numpy as np

a = np.array([1,2,3])
b = np.array(([1,2,3],[4,5,6]))
b1 = np.array(([1,2,3],[4,5,6]))
c = np.array(([1,2,3],[4,5,6],[7,8,9]))
d = np.array(([1,2,3,4],[3,4,5,6]))


print(a) => [1,2,3]
print(a.ndim) => 1
print(a.itemsize) => 4
print(a.dtype) => int32
print(a.size) => 3
print(a.shape) => (3,)
print(a.max()) => 3
print(a.min() => 1
print(a.sum()) => 6

print(b) => [[1,2,3]
             [4,5,6]]
print(b.ndim) => 2
print(b.size) => 6
print(b.shape) => (2,3)
print(b.sum(axis=0)) => [5,7,9]
print(b.sum(axis=1)) => [6,15]
print(np.sqrt(b)) => [[1.         1.41421356 1.73205081]
                      [2.         2.23606798 2.44948974]]
print(np.std(b)) => 1.707825127659933
print(b+b1) => [[ 2  4  6]
               [ 8 10 12]]
print(b-b1) => [[0 0 0]
               [0 0 0]]
print(b*b1) => [[ 1  4  9]
               [16 25 36]]
print(b/b1) => [[1. 1. 1.]
               [1. 1. 1.]]
print(np.vstack((b,b1))) => [[1 2 3]
                             [4 5 6]
                             [1 2 3]
                             [4 5 6]]
print(np.hstack((b,b1))) => [[1 2 3 1 2 3]
                             [4 5 6 4 5 6]]
print(b.ravel()) => [1,2,3,4,5,6]

print(c) => [[1,2,3]
             [4,5,6]
             [7,8,9]]
print(c.ndim) => 2
print(c.size) => 9
print(c.shape) => (3,3)

print(d) => [[1,2,3,4]
             [3,4,5,6]]
print(d[0,2]) => 3
print(d[0:,3]) => [4,6]
print(d[0:,2]) => [3,5]
print(d[1:,2]) => [5]
d = d.reshape(4,2)
print(d) => [[1,2]
             [3,4]
             [3,4]
             [5,6]]

e = np.array(([1,2,3,4],[3,4,5,6],[7,8,9,10]))
print(e[0:,3]) => [4,6,10]
print(e[0:2,3]) => [4,6]

f = np.linspace(1,3,5)
print(f) => [1.  1.5 2.  2.5 3. ]
f = np.linspace(1,3,10)
print(f) => [1.         1.22222222 1.44444444 1.66666667 1.88888889 2.11111111
2.33333333 2.55555556 2.77777778 3.        ]
 
 
import numpy as np
import matplotlib.pyplot as plt
 
x=np.arange(0,3*np.pi,0.1)
y=np.sin(x)
plt.plot(x,y)
plt.show() => Figure about sin function
 
x=np.arange(0,3*np.pi,0.1)
y=np.cos(x)
plt.plot(x,y)
plt.show() => Figure about cos function
 
ar = np.array([1,2,3])
print(np.exp(ar)) => [ 2.71828183  7.3890561  20.08553692]
print(np.log(ar)) => [0.         0.69314718 1.09861229]
print(np.log2(ar)) => [0.        1.        1.5849625]

print(np.zero((3,4))) => [[0. 0. 0. 0.]
                          [0. 0. 0. 0.]
                          [0. 0. 0. 0.]]

x = np.array([(1,2),(3,4)])
y = np.arange(4).reshape((2,2))
z=x*y
z_dot=np.dot(x,y)
z_dot_2=a.dot(b)
print(z) => [[ 0  2]
             [ 6 12]]
print(z_dot) => [[ 4  7]
                 [ 8 15]]
print(z_dot_2) => [[ 4  7]
                 [ 8 15]]
print(np.argmin(x)) => 0
print(np.argmax(x)) => 3
print(np.mean/average(x)) => 2.5
print(x.mean/average()) => 2.5
print(np.median(x)) => 2.5
print(np.cumsum(x)) => [1 3 6 10]
print(np.diff(x)) =>  [[1]
                       [1]]
print(np.transpose(x)) => [[1 3]
                           [2 4]]
print(np.clip(x,2,3)) => [[2 2]
                          [3 3]]

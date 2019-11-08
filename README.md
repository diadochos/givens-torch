Givens Torch
============

Givens rotation layer implementation in PyTorch.

Example
-------
```python
import torch
import givens

A = torch.eye(3)
R = givens.Rotation(3)
R.theta = torch.FloatTensor([3.1415 / 2, 0., 0.])

print(R(A))
# tensor([[ 4.6329e-05,  1.0000e+00,  0.0000e+00],
#         [-1.0000e+00,  4.6329e-05,  0.0000e+00],
#         [ 0.0000e+00,  0.0000e+00,  1.0000e+00]])
```

Doctest
-------
```sh
$ python givens.py
```

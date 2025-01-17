## Modifications of _params_validation Method on GKP Qudit

# Before

The GKP qubit implementation was designed specifically for a 2-dimensional system (qubit).

The parameter d (dimension of qudit) was fixed to 2, implicitly defining the system as a qubit without support for higher-dimensional systems (qudits).

# Now

The _params_validation method has been extended to support qudits of arbitrary dimensions.

Users can now define the dimension of the GKP system using the parameter d. By default, the value of d is set to 2, maintaining backward compatibility with qubit implementations.

# example
```python
from bosonic.codes.gkp import GKPQudit 

q0 = GKPQudit()
```
q0.params['d'] will have value of 2 by default. To change this 

```python
q0.params['d'] = 5
```

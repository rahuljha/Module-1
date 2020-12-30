# MiniTorch Module 1  

<img src="https://minitorch.github.io/_images/match.png" width="100px">

* Docs: https://minitorch.github.io/

* Overview: https://minitorch.github.io/module1.html

This module requires `operators.py` and `module.py` from Module 0

```
cp ../Module-0/operators.py ../Module-0/module.py minitorch/
```


* Tests:

```
python run_tests.py
```

# My Notes

* Parameters are also Variables as well as inputs. All the intermediate outputs are also Variables.
* In backpropagate in autodiff.py, we only add derivatives to Variables that are leaf nodes, this means Variables that have no function history or are not produced by the result of applying a function on some other Variables. These are the parameters Variables.
* The code in run_scalar.py does batch gradient descent. 
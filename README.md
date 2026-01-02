# Leibniz-s-Rule-
#Leibniz's rule on differentiation under integral sign
In[503]:= (*Define functions*)f[x_, t_] := x^2*t^3
a[t_] := Sin[t]
b[t_] := t^2

(*Apply Leibniz rule*)
result = LeibnizRule[f, a, b, t]

(*Or use direct differentiation*)
result2 = D[Integrate[f[x, t], {x, a[t], b[t]}], t] // Simplify

Out[506]= 2 t^8 - t^3 Cos[t] Sin[t]^2 + 3 t^2 (t^6/3 - Sin[t]^3/3)

Out[507]= t^2 (3 t^6 - t Cos[t] Sin[t]^2 - Sin[t]^3)
# This is a Mathematica code for finding the derivative under the integral sign.

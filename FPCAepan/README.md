
[<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/banner.png" width="888" alt="Visit QuantNet">](http://quantlet.de/)

## [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/qloqo.png" alt="Visit QuantNet">](http://quantlet.de/) **FPCAepan** [<img src="https://github.com/QuantLet/Styleguide-and-FAQ/blob/master/pictures/QN2.png" width="60" alt="Visit QuantNet 2.0">](http://quantlet.de/)

```yaml

Name of Quantlet : FPCAepan

Published in : 'Functional Principal Component Analysis for Derivatives of High-Dimensional Spatial
Curves'

Description : Implements the Epanechnikov kernel function for the local polynomial regression.

Keywords : Epanechnikov kernel, smoothing, nonparametric, function, bandwidth

See also : FPCAgpu, FPCAsimulation, FPCAmultiloc, FPCAsimulate_input, FPCAindividual, FPCAvariance

Author : Heiko Wagner

Submitted : Maria Grith

Input: 
- t: time points

Output: 
- k: kernel function

```


### MATLAB Code:
```matlab
function [k]=FPCAepan(t);
k= 3/4*(1-t.^2);
k((abs(t)-1)>0)=0;
end

```

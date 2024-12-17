{% include head.html %}

# TInvar

The TInvar package provides a set of functions for canonicalization of expressions involving the Riemann tensor.
```Mathematica
<< xAct`TInvar`
DefManifold[M, 4, IndexRange[a, f]];
DefMetric[-1, g[-a, -b], CD];
RiemannSimplify[RiemannCD[a, b, c, d] + RiemannCD[a, c, d, b] + RiemannCD[a, d, b, c]]
```

## Installation

1. To run this package you need to have [xAct](http://www.xact.es/) installed.
2. TInvar is distributed as a Paclet that can be installed using [PacletInstall](https://reference.wolfram.com/language/ref/PacletInstall.html.en). For example, to install the latest version from the Black Hole Perturbation Toolkit Paclet Server:
```Mathematica
PacletSiteRegister["https://pacletserver.bhptoolkit.org", "Black Hole Perturbation Toolkit Paclet Server"]
PacletInstall["TInvar"]
```

## Documentation

Usage examples can be found in the documentation. This is available [online](https://bhptoolkit.org/TInvar/doc/html/guide/TInvar.html) and within the Wolfram Documentation Center by selecting Help &#8594; Wolfram Documentation from then menu and searching for `TInvar`.

## Authors

TInvar was created by:

Kevin Kiely, Barry Wardell, Adrian Ottewill and José M. Martín-García.

It is based on Invar and Invar2, which were created by:

José M. Martín-García, David Yllanes, Renato Portugal and Leon Manssur.

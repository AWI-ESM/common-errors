# JSBACH `sum of cover_fract_pot /= 1`

When initalizing the model with a non-standard FESOM mesh, e.g. for simulations on glacial or tectonic time periods, you will also
need to create a new set of atmospheric boundary conditions.

Using a new JSBACH input file may result in errors which show up like this in the logs:

```
FATAL ERROR in fpc_to_cover_fract_pot:  sum of cover_fract_pot /= 1:   1.100000000000000E-009   1.00000000000000                1
```

You should ensure that the sum of `cover_fract_pot` is 1.

# sensors

Q sensors.ssc.so (R tag wasn't leaked yet) with changes in light sensor values
calculation. 

## Problem
LTR578 reports its values already in lx, but driver still tries 
to convert values to lx and because of that sensitivity of sensor goes to zero.

## Fix
Just make driver to do not perform any calculations on LTR578 values.

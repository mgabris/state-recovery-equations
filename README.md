# state-recovery-equations
Sage code for solving complexity estimate equations for state-recovery attacks on ciphers RC4 and Spritz. 

Details can be found in our [paper -- TODO link]().

## Code organization

Code is organized simply: file [compute.sage](https://github.com/mgabris/state-recovery-equations/blob/master/compute.sage) contains code for solving equations (with exception of Spritz special equations, where more elaborate way is needed) provided how to generate equations, variables used in them and their boundary conditions.

Files **_equations.sage* contain functions to generate equations, variables and boundary conditions for particular equation type. Each file contains brief code to compute complexities from equations.

## Usage

For particular equation, just invoke sage with appropriate file.

```bash
$ ./sage rc4_equations.sage
```

## Worksheet

There is also Sage worksheet file [equations.sws](https://github.com/mgabris/state-recovery-equations/blob/master/equations.sws) containing all above code, it may be easier to experiment there.

# simulink-unwrapper-block

[![View UnWrapper on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/6354-unwrapper)

[![Open in MATLAB Online](https://www.mathworks.com/images/responsive/global/open-in-matlab-online.svg)](https://matlab.mathworks.com/open/github/v1?repo=giampy1969/simulink-unwrapper-block)

Normally, the output of functions that return angles (e.g. atan2) is strictly constrained within the range 0 to 2*pi or within the range -pi to pi.

Therefore, even if the inputs change continuously, the angle will exhibit 2*pi jumps across the limits, which is sometimes undesirable (e.g. when the angle drives a control system).

This block unwraps an input angle to the whole real axis so that it does not make 2*pi jumps anymore.

In order to distinguish jumps from normal behavior, an upper bound on the maximum time derivative of the input is assumed.

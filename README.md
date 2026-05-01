# Asian Option Pricing: MC vs ML

Compares Monte Carlo pricing for arithmetic Asian options with a neural network trained on Monte Carlo data. Monte Carlo becomes more accurate as the number of paths increases but also becomes slower. The neural network produces prices much faster, with a small error.

Result: about 100–700× faster than Monte Carlo at high accuracy, with a small loss in precision.

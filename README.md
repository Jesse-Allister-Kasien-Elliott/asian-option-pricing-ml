# Asian Option Pricing: Monte Carlo vs ML

This project compares methods for pricing European arithmetic Asian options: Monte Carlo (with antithetic variates), binomial path enumeration, and a neural network surrogate model. Monte Carlo provides accurate estimates but scales linearly with the number of simulated paths, while the binomial method scales exponentially in time steps and becomes impractical. A neural network is trained to approximate the pricing function \(f(S_0, K, r, \sigma, T)\), using feature normalization and simple feature engineering.

Results show that the neural network achieves small pricing error (~0.01–0.02) while being orders of magnitude faster than Monte Carlo at high accuracy levels (e.g., ~100–700× speedup vs large-path simulations). This demonstrates the tradeoff between accuracy and computational cost, and the effectiveness of machine learning as a fast surrogate for repeated option pricing.

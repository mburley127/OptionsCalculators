## Option Pricing Models
This repository contains implementations of various option pricing models in Python. The models included are:

1. **Binomial Model**
   - `Binomial.ipynb`: Contains the implementation of the Binomial option pricing model.

   The Binomial Option Pricing Model is a widely used method for valuing options, especially American-style ones. It creates a discrete-time framework by modeling possible future price movements of the underlying asset as a binomial tree. Each node in the tree represents a potential price level, and the model calculates option values at each node by considering upward and downward price movements, risk-free interest rates, and the option's strike price. This approach allows for pricing options with early exercise features and complex conditions, making it a versatile tool in financial markets.

2. **Trinomial Model**
   - `Trinomial.ipynb`: Contains the implementation of the Trinomial option pricing model.

   The Trinomial model is an extension of the Binomial model and uses three possible price movements at each step.

3. **Black-Scholes Model**
   - `BlackScholes.ipynb`: Contains the implementation of the Black-Scholes option pricing model.

   The Black-Scholes model is a continuous-time model used for pricing European-style options.

4. **Bjerksund-Stensland Model**
   - `BjerksundStensland.ipynb`: Contains the implementation of the Bjerksund-Stensland option pricing model.

   The Bjerksund-Stensland model is used to price American options with continuous barriers. It incorporates early exercise and barrier features into the option pricing calculation.






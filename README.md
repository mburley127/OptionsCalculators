## Option Pricing Models
This repository contains implementations of various option pricing models in Python. The models included are:

1. **Binomial Model**
   - `Binomial.ipynb`: Contains the implementation of the Binomial option pricing model.

   The Binomial Option Pricing Model is a widely used method for valuing options, especially American-style ones. It creates a discrete-time framework by modeling possible future price movements of the underlying asset as a binomial tree. Each node in the tree represents a potential price level, and the model calculates option values at each node by considering (denoted as "u") and a downward movement (denoted as "d"), risk-free interest rates, and the option's strike price. This approach allows for pricing options where early exercise is optimal.

2. **Trinomial Model**
   - `Trinomial.ipynb`: Contains the implementation of the Trinomial option pricing model.

   The Trinomial Option Pricing Model is an extension of the Binomial Model that incorporates an additional price movement option at each time step, creating a three-branch tree instead of two. This added branch represents a neutral price movement, where the underlying asset neither increases nor decreases in value (denoted as "m"). The Trinomial Model is advantageous as it can capture more complex price dynamics compared to the Binomial Model, providing a more accurate valuation for options with multiple possible price changes. This approach allows for pricing options where early exercise is optimal.

3. **Black-Scholes Model**
   - `BlackScholes.ipynb`: Contains the implementation of the Black-Scholes option pricing model.

   The Black-Scholes model is a continuous-time model used for pricing European-style options.

4. **Bjerksund-Stensland Model**
   - `BjerksundStensland.ipynb`: Contains the implementation of the Bjerksund-Stensland option pricing model.

   The Bjerksund-Stensland model is used to price American options with continuous barriers. It incorporates early exercise and barrier features into the option pricing calculation.






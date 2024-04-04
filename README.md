## Option Pricing Models
This repository contains implementations of various option pricing models in Python. The models included are:

1. **Binomial Model**
   - `Binomial.ipynb`: Contains the implementation of the Binomial option pricing model.

   The Binomial Option Pricing Model is a widely used method for valuing American options, which are options contracts that can be exercised at any point up until, and including, the expiration date. It creates a discrete-time framework by modeling possible future price movements of the underlying asset as a binomial tree. Each node in the tree represents a potential price level, and the model calculates option values at each node by considering the probability of an upward movement (denoted as "u") and a downward movement (denoted as "d"), risk-free interest rates, and the option's strike price. This approach allows for pricing options where early exercise may be optimal.

2. **Trinomial Model**
   - `Trinomial.ipynb`: Contains the implementation of the Trinomial option pricing model.

   The Trinomial Option Pricing Model is an extension of the Binomial Model that incorporates an additional price movement option at each time step, creating a three-branch tree instead of two. This added branch represents a neutral price movement, where the underlying asset neither increases nor decreases in value, but rather does not change (denoted as "m"). The Trinomial Model is advantageous as it can capture more complex price dynamics compared to the Binomial Model, providing a more accurate valuation for options with multiple possible price changes. This approach allows for pricing options where early exercise may be optimal.

3. **Black-Scholes Model**
   - `BlackScholes.ipynb`: Contains the implementation of the Black-Scholes option pricing model.

   The Black-Scholes Model is used for pricing European options, which are options contracts that can only be exercised at the expiration date. The model assumes that stock prices follow a geometric Brownian motion and that the risk-free interest rate and volatility are constant over the option's lifetime. The code implementation calculates both the theoretical price of a call and put option with the results being stored in a dataframe for future analysis.

4. **Bjerksund-Stensland Model**
   - `BjerksundStensland.ipynb`: Contains the implementation of the Bjerksund-Stensland option pricing model.

   The Bjerksund-Stensland model is an extension of the Black-Scholes model that allows for the valuation of American options. It incorporates additional parameters such as the dividend yield, barrier levels, and cost of carrying the asset. The model is particularly useful for valuing options on assets that pay dividends or when there are constraints on when the option can be exercised. It takes into account the optimal exercise strategy for American options, which allows for the determination of whether early exercise is beneficial based on the underlying asset's price dynamics and the option's features. This model provides a more accurate valuation of American options compared to the Black-Scholes model, especially in the presence of dividends and pricing barriers.

5. **Whitepapers**
   - `BlackScholes_Huang2-3`: Pages 2-3 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Black-Scholes Model. 
   - `Binomial_Huang284-286`: Pages 284-286 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Binomial Model.
   - `BjerksundStensland_Huang104-106`: Pages `104-106 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Bjerksund-Stensland Model.
   - `Numerical-Methods-versus-Bjerksund-and-Stensland-Approximations-for-American-Options-Pricing-.pdf`: Comparative analysis of the Binomial, Trinnomial, and Bjerksund-Stensland models with logic used to construct the Binomial/Trinomial Models.



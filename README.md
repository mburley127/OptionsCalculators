## Option Pricing Models
This repository contains implementations of various option pricing models in Python. The models included are:

1. **Black-Scholes Model**
   - `BlackScholes.ipynb`: Contains the implementation of the Black-Scholes option pricing model.

   The Black-Scholes Model is used for pricing European options, which are options contracts that can only be exercised at the expiration date. The model assumes that stock prices follow a geometric Brownian motion and that the risk-free interest rate and volatility are constant over the option's lifetime. The code implementation calculates both the theoretical price of a call and put option with the results being stored in a dataframe for future analysis.

2. **Black 76 Model**
   - `Black76.ipynb`: Contains the implementation of the Black76 option pricing model.

   The Black 76 Model modifies the Black-Scholes formula to handle the unique characteristics of futures contracts. Unlike the Black-Scholes model, which prices options on underlying assets like stocks, the Black 76 Model prices options on the futures price of a commodity. The key difference lies in the treatment of the underlying asset and its discounting. <br/>
   The european call option value is computed as: <br/>
      C = e^(−rT) * [FN(d_1​)−KN(d_2​)] <br/>
   The european put option value is computed as: <br/>
      P = e^(−rT) * [KN(−d_2​)−FN(−d_1​)] <br/>
   where: <br/>
      d_1​ = [ln(F/K)+(σ^2/2)T​] / (σ*sqrt(t)) <br/>
      d_2 = d_1​ − σ*sqrt(T)

4. **Bjerksund-Stensland Model**
   - `BjerksundStensland.ipynb`: Contains the implementation of the Bjerksund-Stensland option pricing model.

   The Bjerksund-Stensland model is an extension of the Black-Scholes model that allows for the valuation of American options. It incorporates additional parameters such as the dividend yield, barrier levels, and cost of carrying the asset. The model is particularly useful for valuing options on assets that pay dividends or when there are constraints on when the option can be exercised. It takes into account the optimal exercise strategy for American options, which allows for the determination of whether early exercise is beneficial based on the underlying asset's price dynamics and the option's features. This model provides a more accurate valuation of American options compared to the Black-Scholes model, especially in the presence of dividends and pricing barriers.

5. **Whitepapers**
   - `BlackScholes_Huang2-3.pdf`: Pages 2-3 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Black-Scholes Model. 
   - `BjerksundStensland_Huang104-106.pdf`: Pages `104-106 of "THE COMPLETE GUIDE TO Option Pricing Formulas SECOND EDITION" by ESPEN GAARDER HAUG which contains the theory and key equations utilized in the Bjerksund-Stensland Model.
   - `Numerical-Methods-versus-Bjerksund-and-Stensland-Approximations-for-American-Options-Pricing-.pdf`: Comparative analysis of the Binomial, Trinomial, and Bjerksund-Stensland models with logic used to construct the Bjerksund-Stensland Model.



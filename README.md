## Option Pricing Models
This repository contains implementations of various option pricing models in Python. The models included are:

1. **Binomial Model**
   - `binomial_model.py`: Contains the implementation of the Binomial option pricing model.

   The Binomial model is a discrete-time model used for pricing options. It calculates the option price at each step of a binomial tree and is based on the following formulas:

   ![Binomial Model Equations](binomial_equations.png)

2. **Trinomial Model**
   - `trinomial_model.py`: Contains the implementation of the Trinomial option pricing model.

   The Trinomial model is an extension of the Binomial model and uses three possible price movements at each step. It is based on the following equations:

   ![Trinomial Model Equations](trinomial_equations.png)

3. **Black-Scholes Model**
   - `black_scholes_model.py`: Contains the implementation of the Black-Scholes option pricing model.

   The Black-Scholes model is a continuous-time model used for pricing European-style options. It is based on the following formulas:

   ![Black-Scholes Model Equations](black_scholes_equations.png)

4. **Bjerksund-Stensland Model**
   - `bjerkson_stensland_model.py`: Contains the implementation of the Bjerksund-Stensland option pricing model.

   The Bjerksund-Stensland model is used to price American options with continuous barriers. It incorporates early exercise and barrier features into the option pricing calculation. The model is based on the following equations:

   ![Bjerksund-Stensland Model Equations](bjerkson_stensland_equations.png)






# Market_Basket_Analysis

In this repo, we will explore the applications of Market Basket Analysis in calculating the similarities between items in a grocery shopping dataset. Please enjot!

### Software, Tools, and prerequisits

1. Access to Google Colab or some Jupyter Notebook.
2. Basic python programing.
3. Basic modular programming knowledge

### Intro: What is Market Basket Analysis?

This is an algorithm used to uncover combinations of items that occur together frequently in transactions. It is frequently used by retailers to identify items that are related and hence anticipate customer behavior. Below are some examples:

- Walmart realizing Bread and Eggs are frequently bought together so the place them at opposite ends of the store (bakery in front, frozen produce in the back) to ensure the customer spends longer in the store and buys more.

- Spotify recomends you as song based on other users that liten to similar songs in a given time period.
  - Customer A has a playst with 10 songs they frequently listen to.
  - Customer B has a playlist with 10 songs but 9 of those are also in customer A playlist.
  - Based on the Association Rule, Customer B is most likely to also enjoy the $10^{th}$ song on customer A's playlist.
  - Spotify recomends that $10^{th}$ song to Customer B

Some key terms in the Associative Rule are Support, Confidence, and lift. Below are the mathematical representations for two products $(X, Y)$:
$$Support = \frac{frq(X,Y)}{N} $$
$$Confidence = \frac{frq(X,Y)}{frq(X)} $$
$$Lift = \frac{Support}{Supp(X) \* Supp(Y)} $$

### Steps to completing the project

1. Import the necessary modules/ packages needed for this project.
2. Load and Prepare the dataset (this involves ensuring no null values).
3. Visualize the dataset by plotting the top 10 most bought items.
4. Prime the data for modelling.
5. Use the Apyori package for the Assosiative Rule calculation.

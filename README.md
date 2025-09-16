# Original Version
#### Etsy Profitability and Material Loss Study
- The numbers in this study were pulled from a client selling handmade goods on Etsy.
- The details about the orders have been removed form this analysis but the numbers used were real. 
- This project was posted on GitHub with permission from client.

# Etsy Product Profitability and Material Loss Report
This report was used to optimize the pricing and material loss calculations used by a local Etsy store. 
- The numbers in this study were pulled from a client selling handmade goods on Etsy.
- The details about the orders have been removed form this analysis but the numbers used were real. 
- This project was posted on GitHub with permission from client. 

## Features
- Generates synthetic data for test analysis using Panda DataFrames.
- Calculates profit and material loss from order length and width.
- Compares different pricing structure for product and calculates margins for each.
- Generates HTML report for client using Jupyter notebook.

## Findings
### Profit Chart
- The per item profit for this product was between \$50 and \$70 for most items.

![png](images/profit_boxen.png)
### Material Loss vs Num Colors
- As num colors went up material loss went up.
- Material loss did not go up evenly for all orders. 

![png](images/material_loss_vs_num_colors.png)
### Material Loss vs Profit
- As material loss went up profit went down.
- Items with low material loss had a profit between \$40 and \$20 before adjustments

![png](images/material_loss_vs_profit.png)

### Final Thoughts
- Based on the profit vs num_color plots the optimal price for our products is \$40 per order and \$10 extra per color.
- Orders with large number of colors are likely to have higher material loss, but also have a potential for higher profit.
- If the client wants to minimize material loss they should only offer products whose dimensions add up to less than 20.

## Frameworks Versions at (09/16/2025)
- python: 3.13
- pandas: 2.3.2
- numpy: 2.3.2
- seaborn: 0.13.2
- jupyterlab: 4.4.7
- jupyter_client: 8.6.3
- jupyter_core: 5.8.1
- jupyter_server: 2.17.0
# Author 
- Product Profitability Report
- Daniel Levenstein
- Date: 09/16/2025
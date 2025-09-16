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
### Material Loss vs Num Colors
- As num colors went up material loss went up.
- Material loss did not go up evenly for all orders. 

![png](images/material_loss_vs_num_colors.png)
### Profit Chart
Four pricing structures were suggested in this report.

![png](images/profit_chart_comparison.png)

### Price Ratings
- Red Line: color surcharge = \$5 with no limits on order dimensions. (Price1)
- Yellow Line: color surcharge = \$5 and material loss < 1 unit (Price2)
- Orange Line: color surcharge = \$5 and length + width == 19 (Price3)
- Green Line: color surcharge = \$7 and length + width == 19 (Price4)

#### Observations
- Of these 3 pricing schemes price 2, price 3, and price 4 are profitable while price 1 is not.
- Price structure 4 has the highest profit margin.
- Pricing structure 2 and 3 are very similar but price 3 is easier to calculate.

### Suggestions
- Client should charge \$40 per item with a  \$5 - \$7 surcharge per additional color
- Client should limit orders to ones whose length and width <=19
## Final Pricing Chart



<div>

<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>Name</th>
      <th>Min Profit</th>
      <th>Max Profit</th>
      <th>Mean Profit</th>
      <th>Median Profit</th>
      <th>size</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>Price 1</td>
      <td>-28.0</td>
      <td>33.0</td>
      <td>17.31</td>
      <td>25.0</td>
      <td>3190</td>
    </tr>
    <tr>
      <th>1</th>
      <td>Price 2</td>
      <td>-1.0</td>
      <td>33.0</td>
      <td>26.83</td>
      <td>29.0</td>
      <td>2230</td>
    </tr>
    <tr>
      <th>2</th>
      <td>Price 3</td>
      <td>21.0</td>
      <td>33.0</td>
      <td>28.30</td>
      <td>29.0</td>
      <td>1540</td>
    </tr>
    <tr>
      <th>3</th>
      <td>Price 4</td>
      <td>38.5</td>
      <td>59.5</td>
      <td>46.73</td>
      <td>45.5</td>
      <td>1540</td>
    </tr>
  </tbody>
</table>
</div>


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
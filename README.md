
<h1 align="center">💻 Laptop Price Prediction - Algerian Market</h1>

<p align="center">
A Machine Learning project developed entirely using <strong>Google Colab</strong> to estimate
the prices of laptops available in the Algerian market.
</p>

<p align="center">
The dataset mainly focuses on laptops priced up to approximately
<strong>120,000 DZD (12 million centimes)</strong>.
</p>

<hr>

<h2>📖 Overview</h2>

<p>
This project uses several Machine Learning regression algorithms to predict laptop prices based on their hardware specifications.
The models are trained and evaluated using the same dataset, then compared using the
<strong>Root Mean Squared Error (RMSE)</strong> metric to automatically select the best-performing model.
</p>

<p>
The final model predicts the estimated market price of a laptop from its encoded hardware specifications.
</p>

<hr>

<h2>🚀 Technologies</h2>

<ul>
<li>Google Colab</li>
<li>Python 3</li>
<li>Pandas</li>
<li>NumPy</li>
<li>Scikit-learn</li>
<li>Matplotlib</li>
</ul>

<hr>

<h2>🤖 Regression Models</h2>

<ul>
<li>K-Nearest Neighbors (KNN)</li>
<li>Linear Regression</li>
<li>Ridge Regression</li>
<li>Lasso Regression</li>
<li>Decision Tree Regressor</li>
<li>Random Forest Regressor</li>
<li>Gradient Boosting Regressor</li>
</ul>

<hr>

<h2>📊 Model Performance (RMSE)</h2>

<table>
<thead>
<tr>
<th>Algorithm</th>
<th>Parameters</th>
<th>RMSE (DA)</th>
</tr>
</thead>

<tbody>

<tr>
<td>KNN</td>
<td>k=3, metric='manhattan'</td>
<td>4247.97</td>
</tr>

<tr>
<td>Linear Regression</td>
<td>fit_intercept=True</td>
<td>494.71</td>
</tr>

<tr>
<td>Decision Tree</td>
<td>max_depth=8</td>
<td>4601.72</td>
</tr>

<tr>
<td>Random Forest</td>
<td>800 Trees</td>
<td>5098.88</td>
</tr>

<tr>
<td>Gradient Boosting</td>
<td>300 Estimators</td>
<td>2096.82</td>
</tr>

<tr>
<td>Ridge Regression</td>
<td>alpha=1</td>
<td>8548.40</td>
</tr>

<tr>
<td><strong>Lasso Regression ⭐</strong></td>
<td>alpha=0.01</td>
<td><strong>487.47</strong></td>
</tr>

</tbody>
</table>

<p>
✅ <strong>Lasso Regression</strong> achieved the best performance and was selected as the final prediction model.
</p>

<hr>

<h2>📑 Dataset Encoding Reference</h2>

<p>
All categorical features are encoded using numeric values to simplify preprocessing and improve model performance.
The following tables explain the encoding used throughout the dataset.
</p>

<h3>Brand (model)</h3>

<table>
<tr>
<th>Code</th>
<th>Brand</th>
</tr>
<tr><td>1</td><td>Dell</td></tr>
<tr><td>2</td><td>HP</td></tr>
<tr><td>3</td><td>Lenovo</td></tr>
<tr><td>4</td><td>Asus</td></tr>
</table>

<h3>Processor (CPU)</h3>

<table>
<tr>
<th>Code</th>
<th>Processor</th>
</tr>
<tr><td>2</td><td>Intel Core i3</td></tr>
<tr><td>4</td><td>Intel Core i5</td></tr>
<tr><td>6</td><td>Intel Core i7</td></tr>
</table>

<h3>Storage Type (Type_Rom)</h3>

<table>
<tr>
<th>Code</th>
<th>Type</th>
</tr>
<tr><td>0</td><td>HDD</td></tr>
<tr><td>1</td><td>SSD</td></tr>
</table>

<h3>Touch Screen (Tactile)</h3>

<table>
<tr>
<th>Code</th>
<th>Value</th>
</tr>
<tr><td>0</td><td>No</td></tr>
<tr><td>1</td><td>Yes</td></tr>
</table>

<h3>Other Features</h3>

<table>

<tr>
<th>Feature</th>
<th>Description</th>
</tr>

<tr>
<td>generation</td>
<td>CPU generation (e.g. 8 = 8th Generation, 12 = 12th Generation)</td>
</tr>

<tr>
<td>Ram_gb</td>
<td>Installed RAM (GB)</td>
</tr>

<tr>
<td>Storage</td>
<td>Storage Capacity (GB)</td>
</tr>

<tr>
<td>icron_pouce</td>
<td>Screen Size (Inches)</td>
</tr>

<tr>
<td>safety_rate</td>
<td>Device Condition (1–10)</td>
</tr>

<tr>
<td>battery_hours</td>
<td>Battery Life (Hours)</td>
</tr>

<tr>
<td>prix</td>
<td>Laptop Price (DZD)</td>
</tr>

</table>

<hr>

<h2>💻 Prediction Example</h2>

<p><strong>Input:</strong></p>

<table>

<tr><th>Feature</th><th>Value</th></tr>

<tr><td>Brand</td><td>1 (Dell)</td></tr>
<tr><td>CPU</td><td>6 (Intel Core i7)</td></tr>
<tr><td>Generation</td><td>8</td></tr>
<tr><td>RAM</td><td>8 GB</td></tr>
<tr><td>Storage</td><td>256 GB</td></tr>
<tr><td>Storage Type</td><td>1 (SSD)</td></tr>
<tr><td>Screen Size</td><td>15.6"</td></tr>
<tr><td>Touch Screen</td><td>0 (No)</td></tr>
<tr><td>Condition</td><td>9 / 10</td></tr>
<tr><td>Battery Life</td><td>4 Hours</td></tr>

</table>

<h3 align="center">🎯 Predicted Price</h3>

<h2 align="center">66,222 DA</h2>

<hr>

<h2>✨ Features</h2>

<ul>
<li>Predicts laptop prices in the Algerian market.</li>
<li>Compares multiple regression algorithms.</li>
<li>Automatically selects the best-performing model.</li>
<li>Uses standardized feature preprocessing.</li>
<li>Supports prediction using encoded hardware specifications.</li>
<li>Built entirely in Google Colab.</li>
</ul>

<hr>

<h2>👨‍💻 Author</h2>

<p><strong>Zehar Djauhar Tadj Eddine</strong></p>

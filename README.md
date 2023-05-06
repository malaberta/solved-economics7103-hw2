Download Link: https://assignmentchef.com/product/solved-economics7103-hw2
<br>



You have access to imaginary data on an energy-efficiency retrofit program in Atlanta <em>kwh.csv </em>and you are interested in whether the program reduced energy use. In your dataset is the following information:

<table width="556">

 <tbody>

  <tr>

   <td width="73">Variable</td>

   <td width="482">Description</td>

  </tr>

  <tr>

   <td width="73"><em>electricity</em></td>

   <td width="482">kWh of electricity used by the household in the month</td>

  </tr>

  <tr>

   <td width="73"><em>sqft</em></td>

   <td width="482">Square feet of the home</td>

  </tr>

  <tr>

   <td width="73"><em>retrofit</em></td>

   <td width="482">= 1 if the home received a retrofit</td>

  </tr>

  <tr>

   <td width="73"><em>temp</em></td>

   <td width="482">The outdoor average temperature (<sup>◦</sup>F) during the month at the home’s location</td>

  </tr>

 </tbody>

</table>

Table 1: Variable descriptions for homework 1.

After recruiting the households for the program, you assigned them to treatment and control groups. Treatment homes received the retrofits on the first of the month and control homes did not have any work done.

<ol>

 <li>Check for balance between the treatment and control groups using Python. Create a table that displayseach variable’s sample mean, sample standard deviation, and p-values for the two-way t-test between treatment and control group means. Your table should have four columns: one with variable names, one with sample mean and standard deviation for the control group, one with sample mean and standard deviation for the treatment group, and one with the p-value for the difference-in-means test. Does it appear that the randomization worked? If so, what can we say about the simple difference-in-means estimate?</li>

 <li>Provide graphical evidence that the retrofits worked. Plot kernel density plots of the electricity use fortreated group and control group on the same graph using Python. Make sure to label the histogram appropriately.</li>

 <li>Suppose you want to estimate the linear equation <em>Y </em>= <em>βX </em>+ <em>ε </em>where <em>Y </em>is an <em>n </em>× 1 vector of the dependent variable, <em>X </em>is an <em>n</em>×<em>p </em>+ 1 matrix of the predictor variables in table 1 and a column of ones, and is an <em>n</em>× 1 vector of unobserved random error. Use the following methods to estimate <em>β</em><sup>ˆ</sup>, presenting coefficients in a single table with a column for each estimation technique (note I am not requiring that you present confidence intervals):

  <ul>

   <li>OLS by hand. Use the Numpy package in Python to create an array <em>X </em>that is the <em>n</em>×<em>p</em>+1 matrix of the predictor variables in table 1 and a column of ones and an array <em>Y </em>that is the <em>n</em>×1 vector of the dependent variable. Use matrix operations to calculate <em>β</em><sup>ˆ</sup>. Recall that <em>β</em><sup>ˆ </sup>= (<em>X</em><sup>0</sup><em>X</em>)<sup>−1</sup><em>X</em><sup>0</sup><em>Y </em>is the closed-form solution to the least-squares minimization problem.</li>

   <li>OLS by simulated least squares. Use the Scipy.optimize.minimize() function in Python to numerically minimize the sum of squares objective function. Recall that the sum of squares is where <em>y<sub>i </sub></em>and <em>x<sub>i </sub></em>are (1 × 1) and (1 ×<em>p </em>+ 1) vectors respectively.</li>

   <li>OLS using a canned routine. Use the StatsModels package in Python using the OLS routine.</li>

  </ul></li>

</ol>
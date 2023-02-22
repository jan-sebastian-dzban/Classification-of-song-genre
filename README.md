# Classification-of-song-genre
Comparison of methods for classification of song genres using GTZAN Database 

# Predicting using ML Methods
The following algorithms will be used:
-Naive Bayes 
-Stochastic Gradient Descent     
-KNN    
-Decission trees    
-Random Forest    
-Support Vector Machine    
-Logistic Regression

For each metod we calculate accuracy score, classification_report and plot confusion_matrix to explore each method separetly.


# Conclusions

We observe best results for set_test_size=0.2 for every method.

Also, accuracy score for given method are very similar no matter what Scaler we chose. However, we can see that for Logistic Regression, Support Vector Machine, KNN we get better results using StandardScaler  but in some cases for Decission trees  MinMaxScaler is better.

The table below shows methods listed from the worst to the best with range of accuracy_score. From the table, we observe the worst method for our data is Naive Bayes and the best is Support Vector Machine.

<style type="text/css">
.tg  {border-collapse:collapse;border-spacing:0;}
.tg td{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  overflow:hidden;padding:10px 5px;word-break:normal;}
.tg th{border-color:black;border-style:solid;border-width:1px;font-family:Arial, sans-serif;font-size:14px;
  font-weight:normal;overflow:hidden;padding:10px 5px;word-break:normal;}
.tg .tg-0lax{text-align:left;vertical-align:top}
</style>
<table class="tg">
<thead>
  <tr>
    <th class="tg-0lax">Method</th>
    <th class="tg-0lax">range of accuracy_score:</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-0lax">-Naive Bayes</td>
    <td class="tg-0lax">[0.45-0.525]</td>
  </tr>
  <tr>
    <td class="tg-0lax">-Decission trees</td>
    <td class="tg-0lax">[0.48-0.565]</td>
  </tr>
  <tr>
    <td class="tg-0lax">-Stochastic Gradient Descent</td>
    <td class="tg-0lax">[0.55-0.615]</td>
  </tr>
  <tr>
    <td class="tg-0lax">-KNN</td>
    <td class="tg-0lax">[0.565-0.645]</td>
  </tr>
  <tr>
    <td class="tg-0lax">-Logistic Regression</td>
    <td class="tg-0lax">[0.6-0.7]</td>
  </tr>
  <tr>
    <td class="tg-0lax">-Support Vector Machine</td>
    <td class="tg-0lax">[0.635-0.74]</td>
  </tr>
</tbody>
</table>

Our set is quite small (1,000 records) thus accuracy score is in range [0.45-0.67] we assume that above methods will perform better on bigger set thats why we will perform the same operations on 5 second samples (6,000 records) in Notebook3 and compare the results.

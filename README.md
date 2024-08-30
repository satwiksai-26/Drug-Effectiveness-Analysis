# Matplotlib - The Power of Plots

## Background

Pymaceuticals Inc. is a company that has been developing anti-cancer pharmaceuticals. They have been conducting studies for anti-cancer pharmaceuticals, with a test using 249 mice to compare tumour size over 45 days, one of the most common skin cancers-treating SCC. In their comparison, they tested various drug regimens in this report to look at the performance of their drug of interest from Pymaceuticals, Capomulin, as against other treatments.

## Requirements
Afterward, generate all necessary tables and charts for the technical report of the study and concisely summarize the findings of the study to present before the executive team.

## Outcomes
Please see [notebooks](pymaceuticals_starter.ipynb) for more details 

## Initial Planning

Joining relevant DataFrames and dropping the duplicate cases of study data are some of the cleaning steps. This was followed by preparing further analyzed data.
</br>
<img src="images\pie_chart.png" width="30%" height="30%">
</br>
### Summary Statistics
Based on the descriptive statistics table, among the treatments, final tumor sizes of Ramicane, Capomulin, Propriva, Ceftamin, and Infubinol are the least. The least mean value here describes that these are the effective drugs; hence, the size of tumors is reduced.
<table class="dataframe" border="1">
  <thead>
    <tr style="text-align: right;">
      <td>Drug Regimen</td>
      <td>mean</td>
      <td>variance</td>
      <td>standard deviation</td>
      <td>SEM</td>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Capomulin</td>
      <td>40.675741</td>
      <td>24.947764</td>
      <td>4.994774</td>
      <td>0.329346</td>
    </tr>
    <tr>
      <td>Ceftamin</td>
      <td>52.591172</td>
      <td>39.290177</td>
      <td>6.268188</td>
      <td>0.469821</td>
    </tr>
    <tr>
      <td>Infubinol</td>
      <td>52.884795</td>
      <td>43.128684</td>
      <td>6.567243</td>
      <td>0.492236</td>
    </tr>
    <tr>
      <td>Ketapril</td>
      <td>55.235638</td>
      <td>68.553577</td>
      <td>8.279709</td>
      <td>0.603860</td>
    </tr>
    <tr>
      <td>Naftisol</td>
      <td>54.331565</td>
      <td>66.173479</td>
      <td>8.134708</td>
      <td>0.596466</td>
    </tr>
    <tr>
      <td>Placebo</td>
      <td>54.033581</td>
      <td>61.168083</td>
      <td>7.821003</td>
      <td>0.581331</td>
    </tr>
    <tr>
      <td>Propriva</td>
      <td>52.393463</td>
      <td>43.138803</td>
      <td>6.568014</td>
      <td>0.525862</td>
    </tr>
    <tr>
      <td>Ramicane</td>
      <td>40.216745</td>
      <td>23.486704</td>
      <td>4.846308</td>
      <td>0.320955</td>
    </tr>
    <tr>
      <td>Stelasyn</td>
      <td>54.233149</td>
      <td>59.450562</td>
      <td>7.710419</td>
      <td>0.573111</td>
    </tr>
    <tr>
      <td>Zoniferol</td>
      <td>53.236507</td>
      <td>48.533355</td>
      <td>6.966589</td>
      <td>0.516398</td>
    </tr>
  </tbody>
</table>
</br>
Ramicane Effectiveness: In general, the drug of Ramicane was more effective in reducing tumor volume when compared to Capomulin. However, from the bar chart showing timepoints versus drug regimen, it would appear that mice treated under Capomulin slightly showed a better survival rate as opposed to Ramicane mice treated—230 timepoints under Capomulin versus 228 under Ramicane.
</br>
<img src="images\bar_chart.png" width="50%" height="50%">
</br>
Thus, Capomulin may be less dangerous in treating tumors.                  
</br>
<img src="images\line_chart.png" width="50%" height="50%">
</br>
Tumor Volume vs. Weight: The mean tumor size is positively correlated with the weight of the mouse, good by the value of r = 0.84, linearly approximated by the equation. 
</br>
<img src="images\linear_regression.png" width="50%" height="50%">
</br>
Where x Let x = weight of the mouse are y is the mean tumor size. Outliers in Data: From the boxplot analysis, there is only one outlier observed within the Infubinol regimen. That is, outliers cannot affect to a greater extent the statistical analysis used in this work. The information given retains the same meaning and substance as in the 
</br>
<img src="images\box_plot.png" width="50%" height="50%">
</br>

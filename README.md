# Time series prediction 

## Objective 
<p> Our objective is to train a time series forecasting model to anticipate demand ride_value in different parts of Tallinn.</p>
<p>
To do so, we need to make our dataset based on location and time for each day of the week. For the purposes of this task,  and considering that we have one month of data, we choose an hourly time frame for our predictions. 
</p>

<h2>Data</h2>
<p><b>start_date:</b>Time the order made</p>
<p><b>start_lat:</b>Latitude of start point</p>
<p><b>start_lng:</b>Langtitude of start point</p>
<p><b>end_lat:</b>Latitude of Destination point</p>
<p><b>end_lng:</b>Langtitude of Destination point</p>



<h1>Baseline Model</h1>
<p>To achieve our objective, we need a predictive model that can learn the historical patterns and identify recurring events. The LSTM model is chosen for this purpose. Since LSTM blocks keep the historical data in memory and can learn complex pattern, this model has both required properties that make it a good choice.</p> 

<h3><i>Hypothesis</i></h3>
<h4><i>LSTM model can be trained to effectively esimate the ride_value in a given location based on previous patterns</i></h4>

<p>To verify the hypothesis, we randomly choose a grid and use 80% of data for training and 20% of data to test.
Cell below shows the process of training and validating the model.</p>

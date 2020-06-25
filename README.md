# Crude-Oil-Prices-Prediction-With-LSTM--Europe

The average daily settlement price for Brent front-month futures contracts increased by 22% from April to May, the largest percentage increase for any month since March 1999. However, even with this increase, prices remain significantly lower than the first-quarter 2020 average. Several factors likely provided support to crude oil prices. Initial oil consumption data and additional efforts by major oil producers indicate that the oversupply in global oil markets has not been as severe as EIA had forecast in the May STEO. As U.S. states and countries in the Organization of Economic Cooperation and Development (OECD) began to reopen from lockdown, early indicators of petroleum consumption have shown increases from the low April levels. EIA estimates that the global consumption of petroleum and other liquid fuels averaged 82.9 million barrels per day (b/d) in May, up 3.7 million b/d from April consumption and 2.9 million b/d more than forecast in the May STEO.


Citation from Redwood Center for Theoretical Neuroscince (Berkeley University)
---------------------
http://redwood.berkeley.edu

http://redwood.berkeley.edu/vs265/Brian-Cheung-LSTMS.pdf

Overall LSTM Structure
----------------
![](https://www.researchgate.net/profile/Oezal_Yildirim/publication/324056729/figure/fig3/AS:619912796073986@1524810136091/Basic-structure-of-the-BLSTM-network-The-LSTM-nets-at-the-bottom-indicate-the-forward.png)



LSTM Node Anatomy
----------------
![alt text](https://devopedia.org/images/article/217/1055.1569518278.jpg)

How LSTM Param Number is computed?
--------------------------------

1. To decide how to handle the memory each LSTM Cell has <bold>3 Gates</bold>: 
    - input (what to let in), 
    - forget (what to forget) and 
    - output (what to write to the output)
2. LSTM **Cell State** is its **memory**
3. LSTM Hidden State is equivalent to the Cell output:
    - lstm_hidden_state_size (number of neurons = memory cells) = lstm_outputs_size
4. Parameters:
    - weights for the inputs (lstm_inputs_size)
    - weights for the outputs (lstm_outputs_size)
    - bias variable
5.  Result from previous point - for all 3 Gates and for Cell State ( = 4)  
   
    # PARAMETERS=4× LSTM outputs size×(weights LSTM inputs size+weights LSTM outputs size+1 bias variable)

# Output After Applying LSTM Model
![g2](https://user-images.githubusercontent.com/52448964/85660334-24348d80-b6d3-11ea-8235-4a1c9b91378c.png)



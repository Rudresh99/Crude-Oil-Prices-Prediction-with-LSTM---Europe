# Crude-Oil-Prices-Prediction--Europe

![](https://user-images.githubusercontent.com/52448964/85650354-06f7c300-b6c3-11ea-947b-51bd32c88f8f.png)

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


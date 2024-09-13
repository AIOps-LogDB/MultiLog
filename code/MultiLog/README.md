# MultiLog 
 
The code for MultiLog is based on two foundational repositories: **logdeep** (https://github.com/d0ng1ee/logdeep/tree/master/logdeep) and **PLELog** (https://github.com/LeonYang95/PLELog). As a result, there are similarities in their calling methods. The only difference is that we replaced the demo folder from logdeep with a **standalone** folder and added a **cluster** module.

## Related Code File in Paper

standalone/DisLog.py
cluster/MultiLogAnomaly.py

## How To Use

Unlike conventional methods, MultiLog requires two steps for training and prediction:

- First, use standalone/DisLog.py to train each node.
- Then, use the corresponding DisLog.py to make predictions and save the results.
- Next, use cluster/MultiLogAnomaly.py to merge and train the results from individual nodes.
- Finally, use MultiLogAnomaly.py to predict anomalies in the cluster.
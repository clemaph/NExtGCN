use Recbole.

config files in .yaml

four datasets: Amazon-Books\Movielens-1M\Yelp\Gowalla in yaml

run "python run_nextgcn_ml.py" directly

|Parameter |Description|
|  ------  |   ------  |
|embedding_size|64|
| USER\_ID\_FIELD|Specifies the user id field|
|ITEM\_ID\_FIELD|Specifies the user id field|
|RATING\_FIELD|Specify the rating field|
|load\_col|Specifies the column name|
|epoches|$500$, maximum epoch of training|
|train\_batch\_size|4096$, batchsize for training|
|learner|Adam, optimizer|
|learning\_rate| $0.001$, learning rate|
|neg\_sample\_num |$1$, number of negative samples|
|eval\_step|$1$, evalaution times after each training|
|stopping\_step| $10$, steps for training convergence|
|eval\_setting|Rearrange randomly, full sort|
|group\_by\_user|True. Whether to group a user record|
|split\_ratio|$[0.8,0.1,0.1]$, dataset split ratio|
|metrics |["Recall", "MRR","NDCG"]|
|topk| $[20]$, k value|
|valid\_metric|Recall@20|
|eval\_batch\_size|$204800$, batchsize for evaluation|

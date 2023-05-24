# Opinion of 1STEP Cardano Stake Pool

## Summary

Poll Hash: `96861fe7da8d45ba5db95071ed3889ed1412929f33610636c072a4b5ab550211`

We **1STEP** have chosen the option "**`Keep k at 500 and halve minPoolCost to 170 ada`**".

## Reason

### Overall

Our decision focuses on **protecting small pools**. As Cardano grows as a public chain, **decentralization** is critical to the health of the network. It is undesirable for only certain participants to have power and to inhibit the growth of developing participants. However, in the current system of Cardano stake pools, **larger pools tend to grow more easily**. Fortunately, 1STEP is growing with the support of many people, but there are still many wonderful people with enthusiasm for Cardano among the SPOs of smaller pools. I believe it is a prerequisite for Cardano's bright future that not only my pool grows, but that the contributions of such people are duly rewarded.

### Keep k at 500

Regarding the k parameter, we support **keep it at 500**. Increasing `k` would mean lowering the saturation point of the pool, which would essentially encourage a move from large pools to smaller pools, but the reality is that this is not the case. Some SPOs **avoid the saturation point** by **operating multiple pools** in pursuit of profit. Currently, there is no solution to this, and it is expected that the increase in `k` will result in an increase in multiple pools. Since this would mean further weakening of the smaller pools, we are **opposed to increasing k parameter** at this time.

### Decrease Minimum Fixed Cost

We support **decreasing** the minimum fixed cost (`minPoolCost`). The existence of a minimum fixed cost is the primary factor that **reduces the rate of return for small pools** and is the **advantage for delegators choosing large pools**. This becomes easier to understand when you consider the ratio of the reward delegators receives to the number of blocks generated per epoch of the pool. If the fixed cost is `340ADA` and the variable fee is `0%`, we have the following. (Assuming the reward for generating one block is `500ADA`)

| Blocks Generated | Total Reward | Operator Reward | Delegator Reward | Delegator Reward Ratio |
|---:|---:|---:|---:|---:|
| 1 | 500 | 340 | 160 | 32.00% |
| 2 | 1,000 | 340 | 660 | 66.00% |
| 3 | 1,500 | 340 | 1,160 | 77.33% |
| 4 | 2,000 | 340 | 1,660 | 83.00% |
| 5 | 2,500 | 340 | 2,160 | 86.40% |

In a pool with one generated block per epoch, the reward earned by the delegators is `32%` of the total pool reward, which is not even half as much as in a pool with four or five generated blocks. Thus, even with a variable fee of `0%`, the small pool is hardly competitive, and delegators will naturally flow to the large pool. On the other hand, if we assume a fixed cost of `170ADA` and a variable fee of `0%`, we have the following.

| Blocks Generated | Total Reward | Operator Reward | Delegators Reward | Delegators Reward Ratio |
|---:|---:|---:|---:|---:|
| 1 | 500 | 170 | 330 | 66.00% |
| 2 | 1,000 | 170 | 830 | 83.00% |
| 3 | 1,500 | 170 | 1,330 | 88.67% |
| 4 | 2,000 | 170 | 1,830 | 91.50% |
| 5 | 2,500 | 170 | 2,330 | 93.20% |

We can see that the percentage of compensation earned by delegators improved for pools with fewer blocks generated per epoch. We are **in favor of decreasing the minimum fixed cost** at this time, as it would make the smaller pools more competitive.

### Considerations

Minimum fixed cost were introduced from a sustainability perspective **to prevent the network from collapsing** due to pool collapse caused by **heated excessive "low-cost competition"**. Lowering the minimum fixed cost will increase this risk by no small amount. Although the vote this time asked only for a change in parameters, we believe that the introduction of a mechanism such as **minimum variable fee** is necessary to reduce the impact of a decrease in minimum fixed cost on sustainability.

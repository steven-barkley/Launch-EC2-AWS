#Placement Groups 

> Sometimes you want control over the EC2 Instance placement strategy
> That strategy can be defined using placement groups
> When you create a placement group, you specify one of the following strategies for the group:

Cluster Same rack and Same AZ

|Placement group types| Use case | Pros | Cons |
| - | - | - |-|
|Cluster| Big Data Fast complete or Low Latency | Great network 10 Gbps | If rack fails all instances fail |
|Spread| Critical Application or High Availiability|Spanned across different Racks | Limited to 7 instances per AZ|
|Partition| Big Data applications |Instances safe from rack failure | Up to 100s of EC2 instances |

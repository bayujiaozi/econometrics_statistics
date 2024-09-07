# 1. 判断两组数据间（单样本看和mean的差异）的显著性差异：
#sktest diff
#histogram diff
# 2.如果已知计量资料满足(或近似满足)t检验或F检验条件（正态分布&方差齐性），应选t检验或F检验： 
#ttest a == b
#ttest diff == 0
#t-test assumes that the data (or more specifically, the differences between paired observations for a paired t-test) follow a normal distribution. However, this assumption primarily affects small sample sizes. For larger sample sizes (usually over 30 observations), the Central Limit Theorem suggests that the t-test is robust to deviations from normality, meaning the results are still reliable even if the data isn't perfectly normal.
## 如果不符合，使用秩转换的非参数检验：Wilcoxon signed-rank test （For a paired t-test, the equivalent non-parametric test.)
#signrank a = b
#signrank diff

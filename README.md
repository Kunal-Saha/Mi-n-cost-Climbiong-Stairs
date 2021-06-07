# Min-cost-Climbing-Stairs
```
//Full Solution and kindly pls understand the logic and then try to implement it by own .......
class Solution {
public:
    int minCostClimbingStairs(vector<int>& cost) {
        for(int i=2;i<cost.size();i++)
        {
            cost[i]+=min(cost[i-1],cost[i-2]);
        }
        return min(cost[cost.size()-1],cost[cost.size()-2]);
    }
};
```

1. 结果最大长度=nums.length-k+1  
2. 遍历nums, 从每个下标开始找k个数判断是否满足条件(滑动窗口)  
3. 当nums剩余个数不足以找到k个数时结束遍历  
4. 当nums剩余个数足以找到k个数时, 判断连续k个数是否递增  
5. 不递增结束  
6. 递增返回最大值, 不递增返回-1  
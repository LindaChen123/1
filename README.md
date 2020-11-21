# 1
leetcode 第一题 两数之和 
C语言
int* twoSum(int* nums, int numsSize, int target, int* returnSize){
    int *r;//创建一个指针用来承接
    for(int i=0;i<numsSize;i++)
        for(int j=i+1;j<numsSize;j++)
        if(target==nums[i]+nums[j])
        {
            r=(int *)malloc(sizeof(int)*2);//要返回一个数组的话，需要用malloc
            *returnSize=2;//解引用
            r[0]=i;
            r[1]=j;
            return r;
        }
        return r;
}


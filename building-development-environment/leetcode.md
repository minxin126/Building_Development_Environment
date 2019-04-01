# 刷题笔记
![image](https://github.com/minxin126/C_Basic/raw/master/Picture/Image1.png)
![image](https://github.com/minxin126/C_Basic/raw/master/Picture/Image2.png)
```c++
// 需要 GNU gcc 4.8版本以上来编译


//     g++ twoSum.cpp -o a.out
//     ./a.out


//      9 （输入9个数）
//      2 3 5 7 11 13 17 19 23 （9个数）
//      40 （和为40）

//      返回： 7 9  （第7个数 + 第9个数 恰好等于目标40）



#include <bits/stdc++.h>
typedef long long ll;
using namespace std;

const int N = 0;

class Solution {
    public:
        vector<int> twoSum(vector<int> &numbers, int target) {
            int sz = numbers.size();
            vector<int> index;
            for (int i = 0; i < sz; i++)
                for (int j = i + 1; j < sz; j++)
                    if (numbers[i] + numbers[j] == target) {
                        index.push_back(i + 1);
                        index.push_back(j + 1);
                        return index;
                    }

        }


};

int main() {
    Solution s;
    vector<int> in;
    int n, t;
    cin >> n;
    while (n--) {
        cin >> t;
        in.push_back(t);
    }
    cin >> t;
    in = s.twoSum(in, t);
    cout << in[0] << ' ' << in[1] << endl;
    return 0;
}
```
## leetcode刷题要求

1. **第1看懂答案，在自己的机子上把答案调通，把整个程序编译运行出来，并且得到正确的结果，一定要能够成功的顺利的运行。**

2. **第2，能够顺利的提交三道题，并且全部正确的在网上提交通过，知道应该怎么提交，知道自己提交的东西是什么。**
3. **第3，弄一个git仓库，把前30道题，创建成30个文件夹，把自己弄出来的答案全部存好，并且过一段时间就提交一下，要注意规范命名，优雅编码。**

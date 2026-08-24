# LeetCode Hot 100 完整专题分类表

## 一、 哈希表 / 数组 (Hash Table & Array)

> 核心思想：利用空间换时间，通过哈希表实现 $O(1)$ 查找，或利用数组固有顺序特性解决连续区间问题 。

| **题号** | **题目名称**   | **核心算法与数据结构**                      |
| -------- | -------------- | ------------------------------------------- |
| **1**    | 两数之和       | 哈希表速查、$O(1)$ 查找                     |
| **49**   | 字母异位词分组 | 字符串排序 / 哈希映射                       |
| **128**  | 最长连续序列   | 哈希集合 (`unordered_set`)、$O(N)$ 连续判断 |

## 二、 双指针 (Two Pointers)

> 核心思想：针对有序或具有单调性的结构，利用左右指针逼近或快慢指针降低时间复杂度 。

| **题号** | **题目名称**   | **核心算法与数据结构**         |
| -------- | -------------- | ------------------------------ |
| **283**  | 移动零         | 快慢双指针（原地方便元素覆盖） |
| **11**   | 盛最多水的容器 | 对撞双指针、贪心收缩           |
| **15**   | 三数之和       | 排序 + 双指针逼近、去重技巧    |
| **42**   | 接雨水         | 对撞双指针 / 单调栈            |

## 三、 滑动窗口 (Sliding Window)

> 核心思想：维护一个动态的区间窗口，通过左右界移动实现区间统计或单调队列优化 。

| **题号** | **题目名称**               | **核心算法与数据结构**                 |
| -------- | -------------------------- | -------------------------------------- |
| **3**    | 无重复字符的最长子串       | 滑动窗口 + 哈希表记录位置              |
| **438**  | 找到字符串中所有字母异位词 | 定长滑动窗口 + 字符词频统计            |
| **239**  | 滑动窗口最大值             | 变长/定长窗口 + 单调双端队列 (`deque`) |

## 四、 子串与矩阵 (Substrings & Matrices)

> 核心思想：结合前缀和、区间合并以及二维矩阵的降维/原地旋转技巧 。

| **题号** | **题目名称**         | **核心算法与数据结构**           |
| -------- | -------------------- | -------------------------------- |
| **560**  | 和为 K 的子数组      | 前缀和 + 哈希表计数              |
| **76**   | 最小覆盖子串         | 滑动窗口 + 字符频次校验          |
| **53**   | 最大子数组和         | 前缀和 / 动态规划（Kadane 算法） |
| **56**   | 合并区间             | 区间按照左端点排序 + 贪心合并    |
| **189**  | 轮转数组             | 数组三段式翻转 / 环形替换        |
| **238**  | 除自身以外数组的乘积 | 前缀积 + 后缀积数组              |
| **41**   | 缺失的第一个正数     | 原地哈希（置换计数）             |
| **73**   | 矩阵置零             | 二维矩阵标记、状态压缩           |
| **54**   | 螺旋矩阵             | 二维矩阵按层顺时针遍历           |
| **48**   | 旋转图像             | 矩阵转置 + 逐行翻转              |
| **240**  | 搜索二维矩阵 II      | 从右上角/左下角出发的 Z 字形搜索 |

## 五、 链表 (Linked List)

> 核心思想：指针翻转、快慢指针追赶、虚头节点（哨兵）与复杂链表结构设计 。

| **题号** | **题目名称**              | **核心算法与数据结构**                       |
| -------- | ------------------------- | -------------------------------------------- |
| **206**  | 反转链表                  | 迭代指针修改 / 递归                          |
| **141**  | 环形链表                  | 快慢指针（Floyd 判圈法）                     |
| **142**  | 环形链表 II               | 快慢指针找入环节点                           |
| **21**   | 合并两个有序链表          | 双指针归并 + 哨兵头节点                      |
| **2**    | 两数相加                  | 链表模拟进位加法                             |
| **19**   | 删除链表的倒数第 N 个结点 | 快慢双指针（保持固定距离 $N$）               |
| **24**   | 两两交换链表中的节点      | 迭代指针交换 / 递归                          |
| **25**   | K 个一组翻转链表          | 局部链表翻转 + 递归/指针连接                 |
| **138**  | 随机链表的复制            | 哈希映射 / 节点交织复制与拆分                |
| **148**  | 排序链表                  | 归并排序（自顶向下 / 自底向上）              |
| **23**   | 合并 K 个升序链表         | 优先队列（最小堆） / 分治归并                |
| **146**  | LRU 缓存                  | 哈希表 + 双向链表 (`unordered_map` + `list`) |

## 六、 二叉树 (Binary Tree)

> 核心思想：深搜 (DFS)、广搜 (BFS)、前中后序遍历以及自顶向下/自底向上的递归树分治 。

| **题号** | **题目名称**                   | **核心算法与数据结构**              |
| -------- | ------------------------------ | ----------------------------------- |
| **94**   | 二叉树的中序遍历               | DFS 递归 / 栈迭代 / Morris 遍历     |
| **104**  | 二叉树的最大深度               | 递归 DFS / 层序 BFS                 |
| **226**  | 翻转二叉树                     | 递归交换左右子树                    |
| **101**  | 对称二叉树                     | 双树同步 DFS/BFS 递归比较           |
| **543**  | 二叉树的直径                   | 递归求深度 + 后序自底向上汇总       |
| **102**  | 二叉树的层序遍历               | BFS 队列辅助                        |
| **108**  | 将有序数组转换为二分搜索树     | 中点二分 + 递归构建                 |
| **98**   | 验证二叉搜索树                 | 中序遍历单调性 / 范围限定递归       |
| **230**  | 二叉搜索树中第 K 小的元素      | BST 中序遍历剪枝                    |
| **199**  | 二叉树的右视图                 | BFS 层序遍历取尾节点 / 右侧优先 DFS |
| **114**  | 二叉树展开为链表               | 先序遍历 / 后序倒序指针调整         |
| **105**  | 从前序与中序遍历序列构造二叉树 | 分治递归 + 哈希表加速定位中点       |
| **437**  | 路径总和 III                   | 树上 DFS + 前缀和哈希表             |
| **236**  | 二叉树的最近公共祖先           | 后序遍历 DFS 状态汇总               |
| **124**  | 二叉树中的最大路径和           | 树形 DP / 自底向上贡献值递归        |

## 七、 图论与搜索 (Graph & Search)

> 核心思想：网格图 DFS/BFS 搜索、连通性判断、拓扑排序判环 。

| **题号** | **题目名称**       | **核心算法与数据结构**               |
| -------- | ------------------ | ------------------------------------ |
| **200**  | 岛屿数量           | 网格 DFS / BFS 染色 / 并查集         |
| **994**  | 腐烂的橘子         | 多源 BFS（广度优先搜索）             |
| **207**  | 课程表             | 拓扑排序（入度数组 + BFS）/ DFS 判环 |
| **208**  | 实现 Trie (前缀树) | 字典树结构设计与字符节点映射         |

## 八、 回溯 (Backtracking)

> 核心思想：递归树遍历、深度优先搜索 (DFS)、状态恢复（撤销选择）与剪枝优化 。

| **题号** | **题目名称**       | **核心算法与数据结构**           |
| -------- | ------------------ | -------------------------------- |
| **46**   | 全排列             | 回溯 + `visited` 数组标记        |
| **78**   | 子集               | 回溯选择 / 位运算子集枚举        |
| **17**   | 电话号码的字母组合 | 回溯构建字符串                   |
| **39**   | 组合总和           | 回溯 + 剪枝（可重复选取元素）    |
| **22**   | 括号生成           | 回溯 + 左右括号匹配约束剪枝      |
| **79**   | 单词搜索           | 网格图 DFS 回溯 + 现场还原       |
| **131**  | 分割回文串         | 回溯 + 动态规划/双指针预处理回文 |
| **51**   | N 皇后             | 回溯 + 列/对角线按位或数组标记   |

## 九、 二分查找 (Binary Search)

> 核心思想：利用单调性折半查找，或在旋转/局部有序结构中确定二分边界 。

| **题号** | **题目名称**                               | **核心算法与数据结构**                   |
| -------- | ------------------------------------------ | ---------------------------------------- |
| **35**   | 搜索插入位置                               | 标准二分查找（左闭右闭/左闭右开）        |
| **74**   | 搜索二维矩阵                               | 二维坐标展开转换为一维二分               |
| **34**   | 在排序数组中查找元素的第一个和最后一个位置 | 二分查找寻找左右边界                     |
| **33**   | 搜索旋转排序数组                           | 局部有序二分判断                         |
| **153**  | 寻找旋转排序数组中的最小值                 | 旋转点二分搜寻                           |
| **4**    | 寻找两个正序数组的中位数                   | 基于分割线/第 $K$ 小元素的双数组二分查找 |

## 十、 栈与堆 (Stack & Heap)

> 核心思想：利用单调栈处理两侧最近大/小元素，利用优先队列（堆）维护动态 Top K 。

| **题号** | **题目名称**            | **核心算法与数据结构**                                  |
| -------- | ----------------------- | ------------------------------------------------------- |
| **20**   | 有效的括号              | 辅助栈匹配                                              |
| **155**  | 最小栈                  | 双栈设计（数据栈 + 辅助单调递减栈）                     |
| **394**  | 字符串解码              | 双栈（倍数栈 + 字符串栈）处理嵌套递归                   |
| **739**  | 每日温度                | 单调递减栈                                              |
| **84**   | 柱状图中最大的矩形      | 单调递增栈 + 左右边界计算                               |
| **215**  | 数组中的第 K 个最大元素 | 小顶堆 (`priority_queue`) / 快速选择算法 (Quick Select) |
| **347**  | 前 K 个高频元素         | 哈希计数 + 小顶堆 / 桶排序                              |
| **295**  | 数据流的中位数          | 对顶堆（大顶堆 + 小顶堆平衡）                           |

## 十一、 动态规划 (Dynamic Programming)

> 核心思想：划分子问题，定义状态与状态转移方程，解决最优解与方案计数问题 。

| **题号** | **题目名称**   | **核心算法与数据结构**                      |
| -------- | -------------- | ------------------------------------------- |
| **70**   | 爬楼梯         | 一维 DP / 斐波那契状态压缩                  |
| **118**  | 杨辉三角       | 二维数组递推                                |
| **198**  | 打家劫舍       | 一维 DP（选择与不选择状态转移）             |
| **279**  | 完全平方数     | DP 状态转移 / BFS 最短路                    |
| **322**  | 零钱兑换       | 完全背包 DP                                 |
| **139**  | 单词拆分       | 字符串 DP + 哈希集合匹配                    |
| **300**  | 最长递增子序列 | $O(N^2)$ DP / $O(N \log N)$ 贪心 + 二分查找 |
| **152**  | 乘积最大子数组 | DP（维护维护连续最大值与最小值）            |
| **416**  | 分割等和子集   | 0-1 背包 DP（状态压缩）                     |
| **32**   | 最长有效括号   | 栈 / 一维 DP / 左右双向遍历计数             |
| **62**   | 不同路径       | 二维 DP 网格递推 / 组合数学                 |
| **64**   | 最小路径和     | 二维 DP（网格自左上角至右下角）             |
| **5**    | 最长回文子串   | 中心扩散法 / 二维 DP / Manacher 算法        |
| **1143** | 最长公共子序列 | 二维 LCS DP                                 |
| **72**   | 编辑距离       | 二维字符串匹配 DP（插入/删除/替换）         |

## 十二、 贪心算法与技巧 (Greedy & Bit Tricks)

> 核心思想：利用局部最优推出全局最优，或利用位运算解决特定位状态变换。

| **题号** | **题目名称**       | **核心算法与数据结构**                     |
| -------- | ------------------ | ------------------------------------------ |
| **55**   | 跳跃游戏           | 贪心（维护能到达的最远边界）               |
| **45**   | 跳跃游戏 II        | 贪心（按步数统计最远可达边界）             |
| **763**  | 划分字母区间       | 贪心（记录字符最远出现位置 + 边界合并）    |
| **121**  | 买卖股票的最佳时机 | 贪心（维护历史最低价格）                   |
| **136**  | 只出现一次的数字   | 位运算（异或性质 $x \oplus x = 0$）        |
| **169**  | 多数元素           | 摩尔投票法 (Boyer-Moore Voting) / 哈希     |
| **75**   | 颜色分类           | 三指针（荷国国旗问题，双边界交换）         |
| **31**   | 下一个排列         | 找右侧首个下降点 + 翻转与交换              |
| **287**  | 寻找重复数         | 快慢指针（抽屉原理转换为环形链表找入环点） |

-----------

## 模板速查总表

| 模块      | 一句话骨架                                | 必背代表题   |
| :-------- | :---------------------------------------- | :----------- |
| 哈希/数组 | 先查后插；只从序列起点起跳                | 128, 1       |
| 双指针    | 对撞移矮侧；快慢 slow 是写入位            | 15, 42       |
| 滑动窗口  | for r 扩 / while 收；求最小在内更新答案   | 76, 239      |
| 前缀和    | `mp[0]=1`，查 `pre-k` 再登记 `pre`        | 560          |
| 矩阵      | 四边界收缩；转置+翻转                     | 54, 48       |
| 链表      | dummy 哨兵 + 三指针反转                   | 25, 146      |
| 二叉树    | 自底向上返回一侧、答案取两侧              | 124, 102     |
| 图        | 多源全入队 BFS；入度出队数判环            | 994, 207     |
| 回溯      | 选择→递归→撤销；start 传 i 还是 i+1       | 39, 51       |
| 二分      | 只写 lower_bound；右边界 = `lower(t+1)-1` | 34, 33       |
| 单调栈    | 存下标，弹栈时结算，尾加哨兵              | 84           |
| 堆        | Top-K 用反向堆；中位数用对顶堆            | 295, 215     |
| DP        | 完全背包正序，0-1 背包倒序                | 322, 416, 72 |
| 贪心      | 维护"当前层边界"，触界即结算              | 45, 763      |

---------------------

# 红黑树

> **红黑树规则**
>
> 1. 每个节点是红色或黑色。
> 2. 根节点是黑色。
> 3. 所有空叶子节点 `NIL` 都是黑色。
> 4. 红色节点的两个子节点必须是黑色，即不能出现连续红色节点。
> 5. 从任一节点到其所有后代 `NIL` 叶子的路径，都包含相同数量的黑色节点。
> 6. 红黑树首先是二叉搜索树：左子树键值小于当前节点，右子树键值大于当前节点。重复键如何处理由实现自行约定。
>
> 这些规则保证树高为 `O(log n)`，因此查找、插入和删除的时间复杂度都是 `O(log n)`。

    #include <iostream>
    #include <stdexcept>
    
    class RedBlackTree {
    private:
        enum class Color { Red, Black };
    
        struct Node {
            int key;
            Color color;
            Node* left;
            Node* right;
            Node* parent;
        };
    
        Node* root;
        Node* nil;  // 所有空孩子共用的黑色哨兵节点
    
        void leftRotate(Node* x) {
            Node* y = x->right;
            x->right = y->left;
    
            if (y->left != nil) {
                y->left->parent = x;
            }
    
            y->parent = x->parent;
    
            if (x->parent == nil) {
                root = y;
            } else if (x == x->parent->left) {
                x->parent->left = y;
            } else {
                x->parent->right = y;
            }
    
            y->left = x;
            x->parent = y;
        }
    
        void rightRotate(Node* y) {
            Node* x = y->left;
            y->left = x->right;
    
            if (x->right != nil) {
                x->right->parent = y;
            }
    
            x->parent = y->parent;
    
            if (y->parent == nil) {
                root = x;
            } else if (y == y->parent->left) {
                y->parent->left = x;
            } else {
                y->parent->right = x;
            }
    
            x->right = y;
            y->parent = x;
        }
    
        void insertFixup(Node* x) {
            while (x->parent->color == Color::Red) {
                // 父节点在祖父节点左侧
                if (x->parent == x->parent->parent->left) {
                    Node* uncle = x->parent->parent->right;
    
                    // 情况1：父红、叔红，只变色并向上继续
                    if (uncle->color == Color::Red) {
                        x->parent->color = Color::Black;
                        uncle->color = Color::Black;
                        x->parent->parent->color = Color::Red;
                        x = x->parent->parent;
                    } else {
                        // 情况2：左-右，先旋转父节点，转成左-左
                        if (x == x->parent->right) {
                            x = x->parent;
                            leftRotate(x);
                        }
    
                        // 情况3：左-左，变色并旋转祖父节点
                        x->parent->color = Color::Black;
                        x->parent->parent->color = Color::Red;
                        rightRotate(x->parent->parent);
                    }
                } else {
                    // 父节点在祖父节点右侧，操作完全对称
                    Node* uncle = x->parent->parent->left;
    
                    if (uncle->color == Color::Red) {
                        x->parent->color = Color::Black;
                        uncle->color = Color::Black;
                        x->parent->parent->color = Color::Red;
                        x = x->parent->parent;
                    } else {
                        // 情况2：右-左，先旋转父节点，转成右-右
                        if (x == x->parent->left) {
                            x = x->parent;
                            rightRotate(x);
                        }
    
                        // 情况3：右-右，变色并旋转祖父节点
                        x->parent->color = Color::Black;
                        x->parent->parent->color = Color::Red;
                        leftRotate(x->parent->parent);
                    }
                }
            }
    
            root->color = Color::Black;
        }
    
        void destroy(Node* node) {
            if (node == nil) {
                return;
            }
    
            destroy(node->left);
            destroy(node->right);
            delete node;
        }
    
        void printInOrder(Node* node) const {
            if (node == nil) {
                return;
            }
    
            printInOrder(node->left);
            std::cout << node->key
                      << (node->color == Color::Red ? "(R) " : "(B) ");
            printInOrder(node->right);
        }
    
    public:
        RedBlackTree() {
            nil = new Node{0, Color::Black, nullptr, nullptr, nullptr};
            nil->left = nil;
            nil->right = nil;
            nil->parent = nil;
            root = nil;
        }
    
        ~RedBlackTree() {
            destroy(root);
            delete nil;
        }
    
        // 本实现不插入重复键；重复时返回 false。
        bool insert(int key) {
            Node* parent = nil;
            Node* current = root;
    
            while (current != nil) {
                parent = current;
    
                if (key < current->key) {
                    current = current->left;
                } else if (key > current->key) {
                    current = current->right;
                } else {
                    return false;
                }
            }
    
            Node* node = new Node{
                key,
                Color::Red,
                nil,
                nil,
                parent
            };
    
            if (parent == nil) {
                root = node;
            } else if (key < parent->key) {
                parent->left = node;
            } else {
                parent->right = node;
            }
    
            insertFixup(node);
            return true;
        }
    
        bool contains(int key) const {
            Node* current = root;
    
            while (current != nil) {
                if (key == current->key) {
                    return true;
                }
                current = key < current->key
                    ? current->left
                    : current->right;
            }
    
            return false;
        }
    
        void printInOrder() const {
            printInOrder(root);
            std::cout << '\n';
        }
    };
    
    int main() {
        RedBlackTree tree;
    
        for (int value : {10, 5, 15, 1, 7, 6, 20, 30}) {
            tree.insert(value);
        }
    
        tree.printInOrder();
    
        std::cout << std::boolalpha
        std::cout << "contains 7: " << tree.contains(7) << '\n';
        std::cout << "contains 8: " << tree.contains(8) << '\n';
    }

| 情况 |           条件           |                   操作                   |
| :--: | :----------------------: | :--------------------------------------: |
|  1   |        父红、叔红        | 父和叔变黑，祖父变红；从祖父继续向上检查 |
|  2   | 父红、叔黑，节点位于内侧 |    旋转父节点，把折线结构转成直线结构    |
|  3   | 父红、叔黑，节点位于外侧 |       父变黑、祖父变红，再旋转祖父       |

------------

# LRU

> Least Recently Used：哈希表 + 双向链表

    class LRUCache {
        struct Node {
            int key, value;
            Node* prev = nullptr;
            Node* next = nullptr;
            Node(int k, int v) : key(k), value(v) {}
        };
    
    public:
        explicit LRUCache(int capacity) : cap_(capacity) {
            head_ = new Node(0, 0);       // 哨兵
            tail_ = new Node(0, 0);
            head_->next = tail_;
            tail_->prev = head_;
        }
        
        ~LRUCache() {
            Node* p = head_;
            while (p) { Node* nx = p->next; delete p; p = nx; }
        }
    
        LRUCache(const LRUCache&) = delete;              // 有裸指针成员，
        LRUCache& operator=(const LRUCache&) = delete;   // 必须禁用或正确实现拷贝
    
        int get(int key) {
            auto it = map_.find(key);
            if (it == map_.end()) return -1;
            moveToFront(it->second);
            return it->second->value;
        }
    
        void put(int key, int value) {
            auto it = map_.find(key);
            if (it != map_.end()) {
                it->second->value = value;
                moveToFront(it->second);
                return;
            }
            if (static_cast<int>(map_.size()) == cap_) {
                Node* victim = tail_->prev;      // 淘汰尾部
                remove(victim);
                map_.erase(victim->key);         // 关键：必须同步删哈希表项
                delete victim;
            }
            Node* node = new Node(key, value);
            map_[key] = node;
            addFront(node);
        }
    private:
        void remove(Node* n) {
            n->prev->next = n->next;
            n->next->prev = n->prev;
        }
    
        void addFront(Node* n) {
        n->next = head_->next;
        n->prev = head_;
        head_->next->prev = n;
        head_->next = n;
        }
    
        void moveToFront(Node* n) { remove(n); addFront(n); }
    
        int cap_;
        Node* head_;
        Node* tail_;
        std::unordered_map<int, Node*> map_;
    };

-------

#  LFU

> Least Frequently Used：哈希表 + 频率哈希表 + 双向链表

```
class LFUCache {
    struct Node {
        int key, value, freq;
    };
    using ListIt = std::list<Node>::iterator;

public:
    explicit LFUCache(int capacity) : cap_(capacity), minFreq_(0) {}
    
    int get(int key) {
        auto it = nodeMap_.find(key);
        if (it == nodeMap_.end()) return -1;
        touch(it->second);
        return it->second->value;
    }

    void put(int key, int value) {
        if (cap_ <= 0) return;                    // 边界

        auto it = nodeMap_.find(key);
        if (it != nodeMap_.end()) {
            it->second->value = value;
            touch(it->second);
            return;
        }

        if (static_cast<int>(nodeMap_.size()) == cap_) {
            // 淘汰 minFreq 桶的尾节点（该频率下最久未用）
            auto& victimList = freqMap_[minFreq_];
            nodeMap_.erase(victimList.back().key);
            victimList.pop_back();
            if (victimList.empty()) freqMap_.erase(minFreq_);
        }

        freqMap_[1].push_front({key, value, 1});
        nodeMap_[key] = freqMap_[1].begin();
        minFreq_ = 1;                             // 新节点频率为 1
    }
    
private:
    void touch(ListIt node) {
        int f = node->freq;
        auto& oldList = freqMap_[f];
        
        // 把节点从 f 桶搬到 f+1 桶，splice 保持迭代器有效
        auto& newList = freqMap_[f + 1];
        newList.splice(newList.begin(), oldList, node);
        ++node->freq;
        nodeMap_[node->key] = node;               // 迭代器未变，但显式写更清晰

        if (oldList.empty()) {
            freqMap_.erase(f);
            if (minFreq_ == f) ++minFreq_;        // 核心：最小频率只可能 +1
        }
    }

    int cap_;
    int minFreq_;
    std::unordered_map<int, std::list<Node>> freqMap_;   // freq → 节点链表
    std::unordered_map<int, ListIt> nodeMap_;            // key  → 节点位置
}；
```

------

# 双指针与滑动窗口

> Two Pointers & Sliding Window：数组/字符串 + 左右双指针

```
// 通用可变窗口模板
int slidingWindow(const std::string& s) {
    std::unordered_map<char, int> window;
    int left = 0, ans = 0;
    for (int right = 0; right < (int)s.size(); ++right) {
        window[s[right]]++;                 // 扩大窗口
        while (/* 窗口不满足条件 */ window[s[right]] > 1) {
            window[s[left]]--;              // 收缩窗口
            ++left;
        }
        ans = std::max(ans, right - left + 1);
    }
    return ans;
}
```

-------

# 前缀和差分

> Prefix Sum & Difference Array：原数组 + 前缀累加数组 / 差分数组

```
// 和为 k 的子数组个数：前缀和 + 哈希
int subarraySum(std::vector<int>& nums, int k) {
    std::unordered_map<long long, int> cnt{{0, 1}};   // 空前缀，别漏
    long long sum = 0;
    int ans = 0;
    for (int x : nums) {
        sum += x;
        auto it = cnt.find(sum - k);      // 找有多少个前缀使 sum - pre == k
        if (it != cnt.end()) ans += it->second;
        ++cnt[sum];
    }
    return ans;
}
```

-------

# 二分查找

> Binary Search：有序数组 + 左右边界指针（区间折半）

```
// 左闭右开，最通用的写法
int lowerBound(const std::vector<int>& a, int target) {
    int lo = 0, hi = a.size();            // 注意 hi 可以取到 n
    while (lo < hi) {
        int mid = lo + (hi - lo) / 2;     // 防溢出，不写 (lo+hi)/2
        if (a[mid] < target) lo = mid + 1;
        else hi = mid;
    }
    return lo;                            // 第一个 >= target 的位置
}
```

-----

# 链表

> Linked List：节点 + next指针（单向 / 双向 / 环形）

```
// 反转链表，迭代版
ListNode* reverse(ListNode* head) {
    ListNode* prev = nullptr;
    while (head) {
        ListNode* next = head->next;   // 先存后继，否则断链
        head->next = prev;
        prev = head;
        head = next;
    }
    return prev;
}

// 快慢指针找中点 / 判环 / 找环入口
ListNode* detectCycle(ListNode* head) {
    ListNode *slow = head, *fast = head;
    while (fast && fast->next) {
        slow = slow->next;
        fast = fast->next->next;
        if (slow == fast) {                    // 有环
            ListNode* p = head;
            while (p != slow) { p = p->next; slow = slow->next; }
            return p;                          // 环入口
        }
    }
    return nullptr;
}
```

----

# 二叉树

> Binary Tree：节点 + 左右子节点指针（递归栈 / BFS 队列）

```
// 递归框架：想清楚"这个节点该做什么"
// 前序：进入节点时处理     中序：左子树完成后处理     后序：左右都完成后处理

// 迭代中序（面试常考，因为它对应 BST 的有序遍历）
std::vector<int> inorder(TreeNode* root) {
    std::vector<int> out;
    std::stack<TreeNode*> st;
    TreeNode* cur = root;
    while (cur || !st.empty()) {
        while (cur) { st.push(cur); cur = cur->left; }  // 一路向左压栈
        cur = st.top(); st.pop();
        out.push_back(cur->val);
        cur = cur->right;
    }
    return out;
}

// 后序思维：需要子树信息才能决策的题（如求直径、判平衡）
int diameter = 0;
int depth(TreeNode* node) {
    if (!node) return 0;
    int l = depth(node->left), r = depth(node->right);
    diameter = std::max(diameter, l + r);       // 经过当前节点的最长路径
    return std::max(l, r) + 1;                  // 返回给父节点的信息
}
```

-----

# 回溯

> Backtracking：递归调用栈 + 路径数组（选择 / 撤销）

```
void backtrack(std::vector<int>& path, /* 状态 */) {
    if (/* 满足终止条件 */) { result.push_back(path); return; }
    for (/* 每个候选 */) {
        if (/* 剪枝：不合法则跳过 */) continue;
        path.push_back(choice);         // 做选择
        backtrack(path, /* 更新状态 */);
        path.pop_back();                // 撤销选择 ← 回溯的本质
    }
}
```

------

# 动态规划

> Dynamic Programming：状态数组/矩阵 + 状态转移方程

```
// 0-1 背包（一维滚动，注意逆序）
for (int i = 0; i < n; ++i)
    for (int j = W; j >= w[i]; --j)              // 逆序！保证每个物品只用一次
        dp[j] = std::max(dp[j], dp[j - w[i]] + v[i]);

// 完全背包：正序遍历即可（允许重复使用）
for (int i = 0; i < n; ++i)
    for (int j = w[i]; j <= W; ++j)
        dp[j] = std::max(dp[j], dp[j - w[i]] + v[i]);

// LIS，O(n log n)：tails[i] 是长度为 i+1 的上升子序列的最小结尾
int lengthOfLIS(std::vector<int>& nums) {
    std::vector<int> tails;
    for (int x : nums) {
        auto it = std::lower_bound(tails.begin(), tails.end(), x);
        if (it == tails.end()) tails.push_back(x);
        else *it = x;
    }
    return tails.size();
}
```

---

# 单调栈与单调队列

> Monotonic Stack & Deque：栈 / 双端队列（维护单调序列）

```
// 下一个更大元素
std::vector<int> nextGreater(std::vector<int>& nums) {
    std::vector<int> ans(nums.size(), -1);
    std::stack<int> st;                          // 存下标，栈内对应值单调递减
    for (int i = 0; i < (int)nums.size(); ++i) {
        while (!st.empty() && nums[st.top()] < nums[i]) {
            ans[st.top()] = nums[i];             // 找到了 st.top() 的下一个更大
            st.pop();
        }
        st.push(i);
    }
    return ans;
}

// 滑动窗口最大值：单调递减双端队列
std::vector<int> maxSlidingWindow(std::vector<int>& nums, int k) {
    std::deque<int> dq;                          // 存下标
    std::vector<int> ans;
    for (int i = 0; i < (int)nums.size(); ++i) {
        while (!dq.empty() && dq.front() <= i - k) dq.pop_front();  // 出窗
        while (!dq.empty() && nums[dq.back()] <= nums[i]) dq.pop_back();
        dq.push_back(i);
        if (i >= k - 1) ans.push_back(nums[dq.front()]);
    }
    return ans;
}
```

-----

# 堆与 Top-K

> Heap & Top-K：优先队列（最大堆 / 最小堆）

```
// 前 K 个高频元素：小顶堆维护大小 K，O(n log k)
std::vector<int> topKFrequent(std::vector<int>& nums, int k) {
    std::unordered_map<int, int> cnt;
    for (int x : nums) ++cnt[x];

    using P = std::pair<int, int>;   // {freq, num}
    std::priority_queue<P, std::vector<P>, std::greater<P>> pq;  // 小顶堆
    for (auto& [num, c] : cnt) {
        pq.emplace(c, num);
        if ((int)pq.size() > k) pq.pop();   // 弹出最小的，保留 k 个最大
    }
    std::vector<int> ans;
    while (!pq.empty()) { ans.push_back(pq.top().second); pq.pop(); }
    return ans;
}
```

-----

# 图与并查集

> Graph & Union-Find：邻接表/矩阵 + 父节点数组（rank/路径压缩）

```
// 并查集：路径压缩 + 按秩合并，近似 O(1)
class DSU {
    std::vector<int> parent_, rank_;
public:
    explicit DSU(int n) : parent_(n), rank_(n, 0) {
        std::iota(parent_.begin(), parent_.end(), 0);
    }
    int find(int x) {
        if (parent_[x] != x) parent_[x] = find(parent_[x]);  // 路径压缩
        return parent_[x];
    }
    bool unite(int a, int b) {
        int ra = find(a), rb = find(b);
        if (ra == rb) return false;
        if (rank_[ra] < rank_[rb]) std::swap(ra, rb);
        parent_[rb] = ra;
        if (rank_[ra] == rank_[rb]) ++rank_[ra];
        return true;
    }
};

// 拓扑排序（Kahn，BFS 版），同时能检测环
std::vector<int> topoSort(int n, std::vector<std::vector<int>>& adj) {
    std::vector<int> indeg(n, 0);
    for (auto& es : adj) for (int v : es) ++indeg[v];

    std::queue<int> q;
    for (int i = 0; i < n; ++i) if (indeg[i] == 0) q.push(i);

    std::vector<int> order;
    while (!q.empty()) {
        int u = q.front(); q.pop();
        order.push_back(u);
        for (int v : adj[u]) if (--indeg[v] == 0) q.push(v);
    }
    return order.size() == (size_t)n ? order : std::vector<int>{};  // 有环则为空
}
```

-------

# 生产者与消费者

> Producer-Consumer：有界队列 + 互斥锁 + 条件变量/信号量

```
template <typename T>
class BlockingQueue { 
public: 
    explicit BlockingQueue(size_t maxSize) : maxSize_(maxSize) {} 

    // 阻塞式生产
    bool push(T item) { 
        std::unique_lock<std::mutex> lk(mtx_); 
        notFull_.wait(lk, [this] { return queue_.size() < maxSize_ || closed_; }); 
        if (closed_) return false; 
        queue_.push(std::move(item)); 
        lk.unlock();                    // 先解锁再通知，减少唤醒后立即阻塞
        notEmpty_.notify_one(); 
        return true; 
    } 

    // 阻塞式消费，返回 false 表示队列已关闭且排空
    bool pop(T& out) { 
        std::unique_lock<std::mutex> lk(mtx_); 
        notEmpty_.wait(lk, [this] { return !queue_.empty() || closed_; }); 
        if (queue_.empty()) return false;          // closed_ 且已排空
        out = std::move(queue_.front()); 
        queue_.pop(); 
        lk.unlock(); 
        notFull_.notify_one(); 
        return true; 
    }

    // 带超时
    bool popFor(T& out, std::chrono::milliseconds timeout) { 
        std::unique_lock<std::mutex> lk(mtx_); 
        if (!notEmpty_.wait_for(lk, timeout, 
                [this] { return !queue_.empty() || closed_; })) { 
            return false;                          // 超时
        } 
        
        if (queue_.empty()) return false; 
        
        out = std::move(queue_.front()); 
        queue_.pop(); 
        lk.unlock(); 
        notFull_.notify_one(); 
        return true; 
    } 
    
    // 优雅关闭：唤醒所有等待者
    void close() { 
        { 
            std::lock_guard<std::mutex> lk(mtx_); 
            closed_ = true; 
        } 
        notEmpty_.notify_all(); 
        notFull_.notify_all(); 
    } 
    
private: 
        size_t maxSize_; 
        bool closed_ = false; 
        std::queue<T> queue_; 
        std::mutex mtx_; 
        std::condition_variable notEmpty_, notFull_; 
}; 

```

---

# LeetCode Hot 100—母题

## 零、ACM 模式的公共 IO 骨架

> 三种ACM 模式的IO

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false);
    cin.tie(nullptr);

    // 读法 A：已知长度 n
    int n; cin >> n;
    vector<int> a(n);
    for (int &x : a) cin >> x;

    // 读法 B：一行不定长数字（最常用）
    string line;
    getline(cin >> ws, line);           // ws 吃掉上一行残留的换行
    vector<int> b;
    { stringstream ss(line); int x; while (ss >> x) b.push_back(x); }

    // 读法 C：一行带 null 的层序序列（建树用）
    vector<string> tok;
    { stringstream ss(line); string s; while (ss >> s) tok.push_back(s); }

    // 输出：数组用空格分隔，二维每行一组
    for (int i = 0; i < (int)b.size(); i++) cout << b[i] << " \n"[i + 1 == (int)b.size()];
    return 0;
}
```

三条硬规则：多组数据用 `while (cin >> n)` 包住；`getline` 前务必 `>> ws`；输出别用 `endl`（每次 flush 会拖慢 IO）。

---

## 一、哈希表 / 数组

### 模板骨架

```
① 计数/去重      → unordered_map<K,int> / unordered_set<K>
② 边遍历边查     → 先查 mp.find(需要的值)，再把当前值插入（避免自己匹配自己）
③ 分组           → 设计"规范化 key"，unordered_map<key, vector<...>>
```

### 代表题：128 最长连续序列（覆盖集合去重 + O(N) 均摊分析）

选它是因为它同时考察"哈希集合"和"如何保证总复杂度 O(N)"这个易错点。

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    string line;
    while (getline(cin, line)) {
        if (line.empty()) continue;
        vector<int> nums;
        { stringstream ss(line); int x; while (ss >> x) nums.push_back(x); }

        unordered_set<int> st(nums.begin(), nums.end());   // 去重 + O(1) 查
        int ans = 0;
        for (int x : st) {
            if (st.count(x - 1)) continue;                 // 关键剪枝：只从"序列起点"起跳
            int cur = x, len = 1;
            while (st.count(cur + 1)) { cur++; len++; }    // 每个数最多被 while 访问一次
            ans = max(ans, len);
        }
        cout << ans << "\n";
    }
    return 0;
}
```

`if (st.count(x-1)) continue;` 是整道题的命脉。没有它，最坏情况每个元素都会向右扫一遍，退化成 O(N²)；有了它，内层 `while` 对整个数据集合计只走 N 步，总复杂度 O(N)。

### 同模块差异片段

**1 两数之和**——先查后插，保证下标不重复：

```cpp
unordered_map<int,int> mp;                 // 值 -> 下标
for (int i = 0; i < n; i++) {
    auto it = mp.find(target - a[i]);
    if (it != mp.end()) { cout << it->second << " " << i << "\n"; break; }
    mp[a[i]] = i;                          // 插入放在查询之后
}
```

**49 字母异位词分组**——核心是设计 key。排序法 O(N·KlogK)，计数法 O(N·K)：

```cpp
// 法一：排序后的字符串作 key
string key = s; sort(key.begin(), key.end());
// 法二：26 位词频拼成签名，更快
string key(26, '0'); for (char c : s) key[c - 'a']++;
mp[key].push_back(s);
```

---

## 二、双指针

### 模板骨架

```
对撞指针：l=0, r=n-1; while (l<r) { 根据某种单调性决定移动哪一侧 }
快慢指针：slow 指向"下一个待写入位置"，fast 负责扫描
```

对撞指针能成立的前提永远是：**移动某一侧不会丢掉最优解**（贪心可证）。

### 代表题：15 三数之和（覆盖排序 + 对撞 + 三层去重）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    string line;
    while (getline(cin, line)) {
        if (line.empty()) continue;
        vector<int> a;
        { stringstream ss(line); int x; while (ss >> x) a.push_back(x); }
        sort(a.begin(), a.end());
        int n = a.size();
        vector<array<int,3>> res;

        for (int i = 0; i < n - 2; i++) {
            if (a[i] > 0) break;                       // 剪枝：最小的已 >0
            if (i > 0 && a[i] == a[i-1]) continue;     // 去重①：固定位不取重复值
            int l = i + 1, r = n - 1;
            while (l < r) {
                long long s = (long long)a[i] + a[l] + a[r];
                if (s < 0) l++;
                else if (s > 0) r--;
                else {
                    res.push_back({a[i], a[l], a[r]});
                    while (l < r && a[l] == a[l+1]) l++;  // 去重②：左指针
                    while (l < r && a[r] == a[r-1]) r--;  // 去重③：右指针
                    l++; r--;
                }
            }
        }
        for (auto &t : res) cout << t[0] << " " << t[1] << " " << t[2] << "\n";
        if (res.empty()) cout << "-\n";
    }
    return 0;
}
```

三处去重的位置不能混：`i > 0 && a[i] == a[i-1]` 是"和前一个已用过的比"，写成 `a[i] == a[i+1]` 会直接漏掉 `[-1,-1,2]` 这类答案。

### 同模块差异片段

**11 盛最多水的容器**——移动矮的那一侧（移动高的一侧面积必不增）：

```cpp
int l = 0, r = n - 1, ans = 0;
while (l < r) {
    ans = max(ans, min(h[l], h[r]) * (r - l));
    h[l] < h[r] ? l++ : r--;
}
```

**42 接雨水**——同为对撞，但维护的是两侧前缀最大值；哪边的最大值小，哪边的水量就已确定：

```cpp
int l = 0, r = n - 1, lm = 0, rm = 0; long long ans = 0;
while (l < r) {
    lm = max(lm, h[l]); rm = max(rm, h[r]);
    if (lm < rm) ans += lm - h[l++];
    else         ans += rm - h[r--];
}
```

**283 移动零**——快慢指针的标准写法，`slow` 是写入位：

```cpp
int slow = 0;
for (int fast = 0; fast < n; fast++)
    if (a[fast] != 0) swap(a[slow++], a[fast]);
```

---

## 三、滑动窗口

### 模板骨架（背下来这一套，3 / 438 / 76 / 209 全通用）

```cpp
init 窗口统计量;
int l = 0;
for (int r = 0; r < n; r++) {
    加入 s[r] 更新统计量;
    while (窗口不合法 或 已可收缩求最优) {
        更新答案（求最小时在这里更新）;
        移出 s[l++] 更新统计量;
    }
    更新答案（求最大时在这里更新）;
}
```

求**最大**窗口 → `while` 条件是"不合法"，答案在循环外更新；求**最小**窗口 → `while` 条件是"已合法"，答案在循环内更新。这是唯一的分叉点。

### 代表题：76 最小覆盖子串（滑窗里最完整的一道）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    string s, t;
    while (cin >> s >> t) {
        unordered_map<char,int> need, win;
        for (char c : t) need[c]++;

        int valid = 0;                       // 已"达标"的字符种类数
        int l = 0, start = 0, len = INT_MAX;
        for (int r = 0; r < (int)s.size(); r++) {
            char c = s[r];
            if (need.count(c)) {
                win[c]++;
                if (win[c] == need[c]) valid++;   // 必须是 == ，不能是 >=
            }
            while (valid == (int)need.size()) {   // 已合法，尝试收缩
                if (r - l + 1 < len) { len = r - l + 1; start = l; }
                char d = s[l++];
                if (need.count(d)) {
                    if (win[d] == need[d]) valid--;  // 先判后减，顺序不能反
                    win[d]--;
                }
            }
        }
        cout << (len == INT_MAX ? "" : s.substr(start, len)) << "\n";
    }
    return 0;
}
```

两个高频翻车点：`win[c] == need[c]` 用 `==` 而非 `>=`，否则 `valid` 会被重复累加；收缩时"先比较再自减"，反过来 `valid` 永远减不动。

### 同模块差异片段

**3 无重复字符的最长子串**——统计量退化为"字符是否出现"：

```cpp
vector<int> cnt(128, 0); int l = 0, ans = 0;
for (int r = 0; r < n; r++) {
    cnt[s[r]]++;
    while (cnt[s[r]] > 1) cnt[s[l++]]--;   // 不合法就收缩
    ans = max(ans, r - l + 1);
}
```

**438 找异位词**——定长窗口，窗口满了就整体比较词频：

```cpp
vector<int> need(26,0), win(26,0);
for (char c : p) need[c-'a']++;
int k = p.size();
for (int r = 0; r < (int)s.size(); r++) {
    win[s[r]-'a']++;
    if (r >= k) win[s[r-k]-'a']--;         // 固定长度，左端自动弹出
    if (r >= k-1 && win == need) cout << r-k+1 << " ";
}
```

### 单调队列：239 滑动窗口最大值

窗口内求极值不能用普通统计量，要用**单调递减双端队列存下标**：

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n, k;
    while (cin >> n >> k) {
        vector<int> a(n); for (int &x : a) cin >> x;
        deque<int> dq;                                     // 存下标，值单调递减
        for (int i = 0; i < n; i++) {
            while (!dq.empty() && dq.front() <= i - k) dq.pop_front();   // 队首过期
            while (!dq.empty() && a[dq.back()] <= a[i]) dq.pop_back();   // 队尾比我小就没用了
            dq.push_back(i);
            if (i >= k - 1) cout << a[dq.front()] << " \n"[i == n-1];
        }
    }
    return 0;
}
```

队列存下标而非值，是为了能用 `dq.front() <= i - k` 判过期。求最小值只需把 `<=` 改成 `>=`。

---

## 四、子串与矩阵

### 4.1 前缀和 + 哈希：560 和为 K 的子数组

模板思想：`区间和(l..r) = pre[r] - pre[l-1]`，把"找区间"转成"找历史前缀和"。

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n, k;
    while (cin >> n >> k) {
        vector<int> a(n); for (int &x : a) cin >> x;
        unordered_map<long long,int> mp;
        mp[0] = 1;                       // 空前缀，处理"从下标 0 开始"的子数组
        long long pre = 0; int ans = 0;
        for (int x : a) {
            pre += x;
            auto it = mp.find(pre - k);  // 查历史，不查自己
            if (it != mp.end()) ans += it->second;
            mp[pre]++;                   // 查完再登记
        }
        cout << ans << "\n";
    }
    return 0;
}
```

`mp[0] = 1` 和"先查后登记"缺一不可。注意本题含负数，不能用滑动窗口。

**437 路径总和 III** 就是这个模板搬到树上：DFS 进入节点时 `mp[pre]++`，回溯时 `mp[pre]--`，保证哈希表里只有当前根到该点这条链上的前缀和。

### 4.2 矩阵模拟：54 螺旋矩阵（四边界收缩模板）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int m, n;
    while (cin >> m >> n) {
        vector<vector<int>> g(m, vector<int>(n));
        for (auto &row : g) for (int &x : row) cin >> x;

        int top = 0, bot = m - 1, lft = 0, rgt = n - 1;
        vector<int> res;
        while (top <= bot && lft <= rgt) {
            for (int j = lft; j <= rgt; j++) res.push_back(g[top][j]);
            top++;
            for (int i = top; i <= bot; i++) res.push_back(g[i][rgt]);
            rgt--;
            if (top <= bot) { for (int j = rgt; j >= lft; j--) res.push_back(g[bot][j]); bot--; }
            if (lft <= rgt) { for (int i = bot; i >= top; i--) res.push_back(g[i][lft]); top_: ; lft++; }
        }
        for (int i = 0; i < (int)res.size(); i++) cout << res[i] << " \n"[i+1 == (int)res.size()];
    }
    return 0;
}
```

后两个方向前面的 `if` 判断是必需的，否则单行或单列矩阵会被重复遍历。

### 同模块其他题的核心片段

**48 旋转图像**（顺时针 90° = 主对角线转置 + 每行翻转）：

```cpp
for (int i = 0; i < n; i++) for (int j = i+1; j < n; j++) swap(g[i][j], g[j][i]);
for (auto &row : g) reverse(row.begin(), row.end());
```

**189 轮转数组**（三段翻转，O(1) 空间）：

```cpp
k %= n;
reverse(a.begin(), a.end());
reverse(a.begin(), a.begin() + k);
reverse(a.begin() + k, a.end());
```

**238 除自身以外的乘积**（前缀积存答案，后缀积用变量滚动）：

```cpp
vector<int> res(n, 1);
for (int i = 1; i < n; i++) res[i] = res[i-1] * a[i-1];
int suf = 1;
for (int i = n-1; i >= 0; i--) { res[i] *= suf; suf *= a[i]; }
```

**41 缺失的第一个正数**（原地哈希：让 `a[i] == i+1`）：

```cpp
for (int i = 0; i < n; i++)
    while (a[i] > 0 && a[i] <= n && a[a[i]-1] != a[i]) swap(a[i], a[a[i]-1]);
for (int i = 0; i < n; i++) if (a[i] != i+1) { cout << i+1; break; }
```

循环条件写 `a[a[i]-1] != a[i]` 而不是 `a[i] != i+1`，是为了在有重复值时避免死循环。

**56 合并区间**（按左端点排序后贪心）：

```cpp
sort(v.begin(), v.end());
vector<pair<int,int>> res;
for (auto &p : v) {
    if (!res.empty() && p.first <= res.back().second) res.back().second = max(res.back().second, p.second);
    else res.push_back(p);
}
```

**240 搜索二维矩阵 II**（从右上角出发，每步排除一行或一列）：

```cpp
int i = 0, j = n - 1;
while (i < m && j >= 0) {
    if (g[i][j] == target) { found; break; }
    g[i][j] > target ? j-- : i++;
}
```

---

## 五、链表

### ACM 模式必备：建链表 / 打印链表

```cpp
struct ListNode {
    int val; ListNode *next;
    ListNode(int v) : val(v), next(nullptr) {}
};

ListNode* buildList(const vector<int>& a) {
    ListNode dummy(0), *p = &dummy;
    for (int x : a) { p->next = new ListNode(x); p = p->next; }
    return dummy.next;
}
void printList(ListNode* h) {
    for (; h; h = h->next) cout << h->val << (h->next ? " " : "\n");
    cout << (h ? "" : "");
}
```

**哨兵节点（dummy）** 是链表题的通用解药：只要头节点可能被删除或替换，就先挂一个 dummy。

### 代表题：25 K 个一组翻转链表（覆盖 206 反转 + 哨兵 + 分段拼接）

```cpp
#include <bits/stdc++.h>
using namespace std;
struct ListNode { int val; ListNode* next; ListNode(int v):val(v),next(nullptr){} };

ListNode* reverseKGroup(ListNode* head, int k) {
    ListNode dummy(0); dummy.next = head;
    ListNode* groupPrev = &dummy;                  // 每组的前驱

    while (true) {
        ListNode* kth = groupPrev;                 // 找本组第 k 个节点
        for (int i = 0; i < k && kth; i++) kth = kth->next;
        if (!kth) break;                           // 不足 k 个，保持原序

        ListNode* groupNext = kth->next;
        ListNode* prev = groupNext, *cur = groupPrev->next, *nxt;
        for (int i = 0; i < k; i++) {              // 标准反转，初始 prev 指向下一组
            nxt = cur->next; cur->next = prev;
            prev = cur; cur = nxt;
        }
        ListNode* newTail = groupPrev->next;       // 原组头翻转后变尾
        groupPrev->next = kth;                     // kth 变新组头
        groupPrev = newTail;
    }
    return dummy.next;
}

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    string line;
    while (getline(cin, line)) {
        if (line.empty()) continue;
        vector<int> a; { stringstream ss(line); int x; while (ss >> x) a.push_back(x); }
        int k; cin >> k; cin.ignore();
        ListNode dummy(0), *p = &dummy;
        for (int x : a) { p->next = new ListNode(x); p = p->next; }
        ListNode* h = reverseKGroup(dummy.next, k);
        for (; h; h = h->next) cout << h->val << (h->next ? ' ' : '\n');
    }
    return 0;
}
```

把反转的初始 `prev` 直接设成 `groupNext`，就省掉了"反转完再接后半段"的额外操作。**206 反转链表**就是把 `prev` 初始设为 `nullptr` 的退化版。

### 快慢指针：141 / 142 环形链表

```cpp
ListNode *slow = head, *fast = head;
while (fast && fast->next) {
    slow = slow->next; fast = fast->next->next;
    if (slow == fast) {                    // 有环
        ListNode* p = head;                // 142：从头和相遇点同速前进
        while (p != slow) { p = p->next; slow = slow->next; }
        return p;                          // 入环点
    }
}
return nullptr;
```

结论来自 `2(a+b) = a+b+k·L` ⟹ `a = k·L - b`，即从头走 a 步与从相遇点走 a 步必在入环点会合。**19 删除倒数第 N 个**同样是快慢指针，让 fast 先走 N+1 步（配合 dummy）再同步。

### 146 LRU 缓存（哈希表 + 双向链表）

```cpp
#include <bits/stdc++.h>
using namespace std;

class LRUCache {
    int cap;
    list<pair<int,int>> lst;                                   // 头部最新，尾部最旧
    unordered_map<int, list<pair<int,int>>::iterator> mp;      // key -> 链表迭代器
public:
    LRUCache(int c) : cap(c) {}
    int get(int k) {
        auto it = mp.find(k);
        if (it == mp.end()) return -1;
        lst.splice(lst.begin(), lst, it->second);              // O(1) 移到头部，迭代器不失效
        return it->second->second;
    }
    void put(int k, int v) {
        auto it = mp.find(k);
        if (it != mp.end()) {
            it->second->second = v;
            lst.splice(lst.begin(), lst, it->second);
            return;
        }
        if ((int)lst.size() == cap) { mp.erase(lst.back().first); lst.pop_back(); }
        lst.push_front({k, v});
        mp[k] = lst.begin();
    }
};

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int cap, q;
    while (cin >> cap >> q) {
        LRUCache lru(cap);
        while (q--) {
            string op; cin >> op;
            if (op == "get") { int k; cin >> k; cout << lru.get(k) << "\n"; }
            else { int k, v; cin >> k >> v; lru.put(k, v); }
        }
    }
    return 0;
}
```

`list::splice` 是这题的关键：它只改指针，不移动元素，所以 `mp` 里存的迭代器始终有效。面试若要求手写双向链表，把 `list` 换成自己的 `Node{prev,next}` 加两个哨兵 head/tail 即可，逻辑完全一致。

### 其余链表题的一句话骨架

- **21 合并两个有序链表**：dummy + 双指针取小者接上，末尾接剩余。
- **23 合并 K 个**：`priority_queue<ListNode*, vector<ListNode*>, cmp>` 存每条链表头，O(N log K)；或两两分治归并。
- **148 排序链表**：快慢指针找中点断开 + 归并；要 O(1) 空间就自底向上按步长 1,2,4… 归并。
- **138 复制随机链表**：节点交织法——`A->A'->B->B'`，`A'->random = A->random->next`，最后拆分，O(1) 额外空间。

---

## 六、二叉树

### ACM 模式建树 / 遍历模板

```cpp
struct TreeNode { int val; TreeNode *left, *right; TreeNode(int v):val(v),left(nullptr),right(nullptr){} };

TreeNode* buildTree(const vector<string>& v) {          // 层序，空用 "null"
    if (v.empty() || v[0] == "null") return nullptr;
    TreeNode* root = new TreeNode(stoi(v[0]));
    queue<TreeNode*> q; q.push(root);
    size_t i = 1;
    while (!q.empty() && i < v.size()) {
        TreeNode* cur = q.front(); q.pop();
        if (i < v.size() && v[i] != "null") { cur->left  = new TreeNode(stoi(v[i])); q.push(cur->left);  } i++;
        if (i < v.size() && v[i] != "null") { cur->right = new TreeNode(stoi(v[i])); q.push(cur->right); } i++;
    }
    return root;
}
```

三种遍历骨架：

```cpp
// 递归（前/中/后只是 visit 位置不同）
void dfs(TreeNode* r) { if (!r) return; /*前*/ dfs(r->left); /*中*/ dfs(r->right); /*后*/ }

// 中序迭代（94）
stack<TreeNode*> st; TreeNode* cur = root;
while (cur || !st.empty()) {
    while (cur) { st.push(cur); cur = cur->left; }
    cur = st.top(); st.pop();
    visit(cur);
    cur = cur->right;
}

// Morris 中序，O(1) 空间：用右指针空位建"线索"
while (cur) {
    if (!cur->left) { visit(cur); cur = cur->right; }
    else {
        TreeNode* pre = cur->left;
        while (pre->right && pre->right != cur) pre = pre->right;
        if (!pre->right) { pre->right = cur; cur = cur->left; }     // 建线索
        else { pre->right = nullptr; visit(cur); cur = cur->right; } // 拆线索
    }
}
```

### 代表题 A：102 层序遍历（BFS 分层模板）

```cpp
#include <bits/stdc++.h>
using namespace std;
struct TreeNode { int val; TreeNode *left,*right; TreeNode(int v):val(v),left(nullptr),right(nullptr){} };

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    string line;
    while (getline(cin, line)) {
        if (line.empty()) continue;
        vector<string> v; { stringstream ss(line); string s; while (ss >> s) v.push_back(s); }
        // ---- 建树（同上，略写为内联）----
        TreeNode* root = nullptr;
        if (!v.empty() && v[0] != "null") {
            root = new TreeNode(stoi(v[0]));
            queue<TreeNode*> q; q.push(root); size_t i = 1;
            while (!q.empty() && i < v.size()) {
                TreeNode* c = q.front(); q.pop();
                if (i < v.size() && v[i] != "null") { c->left = new TreeNode(stoi(v[i])); q.push(c->left); } i++;
                if (i < v.size() && v[i] != "null") { c->right= new TreeNode(stoi(v[i])); q.push(c->right);} i++;
            }
        }
        // ---- BFS 分层 ----
        queue<TreeNode*> q; if (root) q.push(root);
        while (!q.empty()) {
            int sz = q.size();                     // 先固化本层节点数，这是分层的关键
            for (int i = 0; i < sz; i++) {
                TreeNode* c = q.front(); q.pop();
                cout << c->val << (i + 1 == sz ? '\n' : ' ');
                if (c->left)  q.push(c->left);
                if (c->right) q.push(c->right);
            }
        }
    }
    return 0;
}
```

`int sz = q.size()` 必须在循环外取一次。**199 右视图**只需在 `i == sz-1` 时输出；**104 最大深度**只需数层数。

### 代表题 B：124 二叉树中的最大路径和（树形 DP 模板）

这是"自底向上返回值 + 全局答案"这一大类的天花板题，掌握它，543 / 543 直径、236 LCA 都是同构的。

```cpp
int ans = INT_MIN;

int gain(TreeNode* r) {              // 返回值：以 r 为端点向上延伸的最大贡献
    if (!r) return 0;
    int l = max(0, gain(r->left));   // 负贡献直接丢弃（不选这条子树）
    int rr = max(0, gain(r->right));
    ans = max(ans, r->val + l + rr); // 在 r 处"拐弯"的路径，只能用于更新答案
    return r->val + max(l, rr);      // 向上返回时只能选一侧，否则不成链
}
```

分清两个量是全部要点：**更新全局答案时可以左右都取（路径在此拐弯）；向父节点返回时只能取一侧（路径必须是链）**。

同构改写：

```cpp
// 543 直径：返回深度，答案取 l + r（边数）
int depth(TreeNode* r){ if(!r) return 0; int l=depth(r->left), r2=depth(r->right); ans=max(ans,l+r2); return max(l,r2)+1; }

// 236 最近公共祖先：返回"这棵子树里找到的 p/q 或 LCA"
TreeNode* lca(TreeNode* r, TreeNode* p, TreeNode* q){
    if (!r || r == p || r == q) return r;
    TreeNode* l = lca(r->left,p,q); TreeNode* rr = lca(r->right,p,q);
    if (l && rr) return r;           // 左右各找到一个 -> 当前就是 LCA
    return l ? l : rr;
}
```

### 其余树题的骨架

- **98 验证 BST**：范围限定递归 `check(r, low, high)`，或中序遍历检查严格递增（用 `long long prev` 防溢出）。
- **230 第 K 小**：中序遍历计数到 K 立即返回，用迭代版可提前 break。
- **105 前序+中序建树**：`unordered_map<val,idx>` 定位根在中序的位置，递归分治，注意左子树长度 = `pos - inL`。
- **108 有序数组转 BST**：取中点作根，左右区间递归。
- **114 展开为链表**：反向后序（右→左→根）记录 `prev`，令 `cur->right = prev, cur->left = nullptr`。

---

## 七、图论与搜索

### 7.1 网格 BFS/DFS 模板

```cpp
int dir[4][2] = {{1,0},{-1,0},{0,1},{0,-1}};
// 越界与访问检查统一写法
if (ni < 0 || ni >= m || nj < 0 || nj >= n || g[ni][nj] != target) continue;
```

### 代表题：994 腐烂的橘子（多源 BFS，覆盖 200 的染色思想）

```cpp
#include <bits/stdc++.h>
using namespace std;
int dir[4][2] = {{1,0},{-1,0},{0,1},{0,-1}};

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int m, n;
    while (cin >> m >> n) {
        vector<vector<int>> g(m, vector<int>(n));
        queue<pair<int,int>> q; int fresh = 0;
        for (int i = 0; i < m; i++)
            for (int j = 0; j < n; j++) {
                cin >> g[i][j];
                if (g[i][j] == 2) q.push({i, j});   // 所有腐烂橘子一起入队 = 多源
                else if (g[i][j] == 1) fresh++;
            }

        int minutes = 0;
        while (!q.empty() && fresh > 0) {
            int sz = q.size();                       // 按层扩散 = 按分钟推进
            for (int k = 0; k < sz; k++) {
                auto [x, y] = q.front(); q.pop();
                for (auto &d : dir) {
                    int nx = x + d[0], ny = y + d[1];
                    if (nx < 0 || nx >= m || ny < 0 || ny >= n || g[nx][ny] != 1) continue;
                    g[nx][ny] = 2; fresh--;
                    q.push({nx, ny});
                }
            }
            minutes++;
        }
        cout << (fresh > 0 ? -1 : minutes) << "\n";
    }
    return 0;
}
```

多源 BFS 的精髓：把所有起点**一次性全部入队**，等价于建了一个虚拟超级源点，一次 BFS 即得所有点到最近源点的距离。**200 岛屿数量**则是单源反复启动：遇到 `1` 就 `ans++` 并 DFS 把整片连通块改成 `0`。

### 7.2 拓扑排序：207 课程表（BFS 入度法）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n, m;                                   // n 门课，m 条依赖
    while (cin >> n >> m) {
        vector<vector<int>> g(n);
        vector<int> indeg(n, 0);
        for (int i = 0; i < m; i++) {
            int a, b; cin >> a >> b;            // 修 a 前必须修 b，即 b -> a
            g[b].push_back(a);
            indeg[a]++;
        }
        queue<int> q;
        for (int i = 0; i < n; i++) if (!indeg[i]) q.push(i);

        int cnt = 0;
        vector<int> order;
        while (!q.empty()) {
            int u = q.front(); q.pop();
            order.push_back(u); cnt++;
            for (int v : g[u]) if (--indeg[v] == 0) q.push(v);
        }
        cout << (cnt == n ? "YES" : "NO") << "\n";   // 出队数 < n 说明有环
        if (cnt == n) for (int i = 0; i < n; i++) cout << order[i] << " \n"[i+1==n];
    }
    return 0;
}
```

判环的判据就一句：**能出队的节点数是否等于 n**。DFS 判环则用三色标记（0 未访问 / 1 在栈中 / 2 已完成），撞到状态 1 即有环。

### 7.3 Trie：208 前缀树

```cpp
struct Trie {
    Trie* ch[26] = {};
    bool end = false;
    void insert(const string& s) {
        Trie* p = this;
        for (char c : s) {
            int i = c - 'a';
            if (!p->ch[i]) p->ch[i] = new Trie();
            p = p->ch[i];
        }
        p->end = true;
    }
    Trie* find(const string& s) {           // 返回前缀终点节点
        Trie* p = this;
        for (char c : s) { int i = c - 'a'; if (!p->ch[i]) return nullptr; p = p->ch[i]; }
        return p;
    }
    bool search(const string& s)     { Trie* p = find(s); return p && p->end; }
    bool startsWith(const string& s) { return find(s) != nullptr; }
};
```

`search` 与 `startsWith` 唯一的区别是要不要检查 `end` 标记。

---

## 八、回溯

### 三类问题的统一模板

```cpp
void backtrack(参数) {
    if (终止条件) { res.push_back(path); return; }
    for (int i = start; i < n; i++) {
        if (剪枝条件) continue / break;
        path.push_back(选择);       // 做选择
        backtrack(下一层参数);       // 递归
        path.pop_back();            // 撤销选择
    }
}
```

三类的分叉点只在**下一层怎么传**：

| 类型                | 代表题       | 循环起点    | 下一层传参    | 去重手段                    |
| :------------------ | :----------- | :---------- | :------------ | :-------------------------- |
| 排列                | 46           | `i = 0`     | 不传 start    | `visited[]` 数组            |
| 子集/组合（不复用） | 78 / 39 变体 | `i = start` | `i + 1`       | `i > start && a[i]==a[i-1]` |
| 组合（可复用）      | 39           | `i = start` | `i`（不加 1） | 同上                        |

### 代表题 A：39 组合总和（含排序剪枝）

```cpp
#include <bits/stdc++.h>
using namespace std;

vector<int> c, path;
vector<vector<int>> res;

void dfs(int start, int rest) {
    if (rest == 0) { res.push_back(path); return; }
    for (int i = start; i < (int)c.size(); i++) {
        if (c[i] > rest) break;              // 已排序，后面只会更大，直接 break
        path.push_back(c[i]);
        dfs(i, rest - c[i]);                 // 传 i：允许重复使用当前元素
        path.pop_back();
    }
}

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n, target;
    while (cin >> n >> target) {
        c.assign(n, 0); for (int &x : c) cin >> x;
        sort(c.begin(), c.end());            // 排序是剪枝的前提
        res.clear(); path.clear();
        dfs(0, target);
        for (auto &v : res) {
            for (int i = 0; i < (int)v.size(); i++) cout << v[i] << " \n"[i+1==(int)v.size()];
        }
    }
    return 0;
}
```

`dfs(i, ...)` 传 `i` 表示可重复选，传 `i+1` 就变成每个元素只用一次（40 题）。有重复元素时再加一行 `if (i > start && c[i] == c[i-1]) continue;` —— 注意是 `i > start` 而非 `i > 0`，含义是"同一层里不选重复值，但不同层可以"。

**46 全排列**只改两处：循环从 0 开始、用 `visited`：

```cpp
for (int i = 0; i < n; i++) {
    if (vis[i]) continue;
    vis[i] = true;  path.push_back(a[i]);
    dfs();
    path.pop_back(); vis[i] = false;
}
```

**78 子集**是"每个节点都是答案"：把 `res.push_back(path)` 放在函数入口而非终止条件里；或直接位运算枚举 `for (int mask = 0; mask < (1<<n); mask++)`。

### 代表题 B：51 N 皇后（棋盘型 + O(1) 冲突判定）

```cpp
#include <bits/stdc++.h>
using namespace std;

int n, cnt;
vector<int> col, dg1, dg2, pos;      // dg1: i+j 主对角; dg2: i-j+n 副对角
vector<vector<string>> res;

void dfs(int r) {
    if (r == n) {
        cnt++;
        vector<string> board(n, string(n, '.'));
        for (int i = 0; i < n; i++) board[i][pos[i]] = 'Q';
        res.push_back(board);
        return;
    }
    for (int c = 0; c < n; c++) {
        if (col[c] || dg1[r + c] || dg2[r - c + n]) continue;   // O(1) 判冲突
        col[c] = dg1[r + c] = dg2[r - c + n] = 1;
        pos[r] = c;
        dfs(r + 1);
        col[c] = dg1[r + c] = dg2[r - c + n] = 0;               // 精确撤销
    }
}

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    while (cin >> n) {
        col.assign(n, 0); dg1.assign(2*n, 0); dg2.assign(2*n, 0); pos.assign(n, 0);
        res.clear(); cnt = 0;
        dfs(0);
        cout << cnt << "\n";
        for (auto &b : res) { for (auto &row : b) cout << row << "\n"; cout << "\n"; }
    }
    return 0;
}
```

按行放置天然保证了行不冲突；同一主对角线上 `i+j` 恒定，同一副对角线上 `i-j` 恒定（加 n 是为了防负下标）。**79 单词搜索**是同一套骨架搬到网格：把 `g[i][j]` 临时改成 `'#'` 作访问标记，回溯时还原。

---

## 九、二分查找

### 模板骨架（推荐只记这一套：左闭右开 + lower_bound 语义）

```cpp
// 求第一个 >= target 的下标（找不到返回 n）
int lower(vector<int>& a, int target) {
    int l = 0, r = a.size();                 // [l, r)
    while (l < r) {
        int m = l + (r - l) / 2;             // 防溢出
        if (a[m] < target) l = m + 1;
        else r = m;
    }
    return l;
}
// 求第一个 > target：把 a[m] < target 改成 a[m] <= target
```

**35 搜索插入位置**的答案就是 `lower(a, target)`，一行搞定。

### 代表题 A：34 查找元素的第一个和最后一个位置

```cpp
#include <bits/stdc++.h>
using namespace std;

int lowerBound(vector<int>& a, int t) {          // 第一个 >= t
    int l = 0, r = a.size();
    while (l < r) { int m = l + (r-l)/2; a[m] < t ? l = m+1 : r = m; }
    return l;
}

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n, t;
    while (cin >> n >> t) {
        vector<int> a(n); for (int &x : a) cin >> x;
        int L = lowerBound(a, t);
        if (L == n || a[L] != t) { cout << "-1 -1\n"; continue; }
        int R = lowerBound(a, t + 1) - 1;        // 第一个 > t 的前一位
        cout << L << " " << R << "\n";
    }
    return 0;
}
```

用 `lower(t+1) - 1` 求右边界，比手写两套边界条件安全得多。

### 代表题 B：33 搜索旋转排序数组（局部有序判定）

```cpp
int search(vector<int>& a, int t) {
    int l = 0, r = a.size() - 1;
    while (l <= r) {
        int m = l + (r - l) / 2;
        if (a[m] == t) return m;
        if (a[l] <= a[m]) {                          // 左半段有序
            if (a[l] <= t && t < a[m]) r = m - 1;    // 目标在有序段内
            else l = m + 1;
        } else {                                     // 右半段有序
            if (a[m] < t && t <= a[r]) l = m + 1;
            else r = m - 1;
        }
    }
    return -1;
}
```

固定套路：**先判断哪半段有序，再判断 target 是否落在那个有序段内**，落在就收缩到该段，否则去另一段。`a[l] <= a[m]` 的等号处理 `l == m` 的情况，不能漏。

**153 找最小值**更简洁，与 `a[r]` 比较即可（和 `a[l]` 比会在无旋转时出错）：

```cpp
int l = 0, r = n - 1;
while (l < r) { int m = l + (r-l)/2; a[m] > a[r] ? l = m+1 : r = m; }
// a[l] 即最小值
```

**4 寻找两个正序数组的中位数**是二分的上限题：在较短数组上二分分割线 `i`，令 `j = (m+n+1)/2 - i`，调整到 `A[i-1] <= B[j] && B[j-1] <= A[i]` 即可，边界用 `INT_MIN/INT_MAX` 哨兵处理。

---

## 十、栈与堆

### 10.1 单调栈模板

```
求"下一个更大元素" → 单调递减栈（栈内从底到顶递减），弹出时结算
求"左右两侧第一个更小" → 单调递增栈
栈里存下标而不是值（这样才能算距离）
```

### 代表题：84 柱状图中最大的矩形（单调栈里最完整的一道）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n;
    while (cin >> n) {
        vector<long long> h(n);
        for (auto &x : h) cin >> x;
        h.push_back(-1);                        // 尾哨兵：强制清空栈，结算所有柱子

        stack<int> st;                          // 存下标，高度单调递增
        long long ans = 0;
        for (int i = 0; i <= n; i++) {
            while (!st.empty() && h[st.top()] >= h[i]) {
                int cur = st.top(); st.pop();
                int left = st.empty() ? -1 : st.top();   // 弹栈后的新栈顶 = 左边界
                ans = max(ans, h[cur] * (i - left - 1)); // 宽度 = 右边界 - 左边界 - 1
            }
            st.push(i);
        }
        cout << ans << "\n";
    }
    return 0;
}
```

被弹出的柱子 `cur`，其**右边第一个更矮的是 i，左边第一个更矮的是弹栈后的新栈顶**，两者同时确定，宽度就是 `i - left - 1`。尾哨兵 `-1` 省掉了循环后的清栈代码。

**739 每日温度**是同一骨架的简化版（结算的是距离而非面积）：

```cpp
stack<int> st;
for (int i = 0; i < n; i++) {
    while (!st.empty() && t[st.top()] < t[i]) { res[st.top()] = i - st.top(); st.pop(); }
    st.push(i);
}
```

**20 有效括号**：左括号入栈，右括号检查栈顶匹配；**155 最小栈**：辅助栈同步压入 `min(当前值, 辅助栈顶)`；**394 字符串解码**：数字栈 + 字符串栈，遇 `[` 压栈清空，遇 `]` 弹栈重复拼接。

### 10.2 堆模板

```cpp
priority_queue<int> maxHeap;                                    // 大顶堆（默认）
priority_queue<int, vector<int>, greater<int>> minHeap;         // 小顶堆
// Top-K 最大 → 维护大小为 K 的小顶堆，堆顶是第 K 大
```

### 代表题：295 数据流的中位数（对顶堆）

```cpp
#include <bits/stdc++.h>
using namespace std;

class MedianFinder {
    priority_queue<int> lo;                                     // 大顶堆，存较小的一半
    priority_queue<int, vector<int>, greater<int>> hi;          // 小顶堆，存较大的一半
public:
    void addNum(int x) {
        lo.push(x);                        // 先无脑进 lo
        hi.push(lo.top()); lo.pop();       // 把 lo 的最大值挪给 hi，保证 lo 所有元素 <= hi
        if (lo.size() < hi.size()) { lo.push(hi.top()); hi.pop(); }  // 再平衡大小
    }
    double findMedian() {
        return lo.size() > hi.size() ? lo.top() : (lo.top() + hi.top()) / 2.0;
    }
};

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int q;
    while (cin >> q) {
        MedianFinder mf;
        cout << fixed << setprecision(1);
        while (q--) {
            string op; cin >> op;
            if (op == "add") { int x; cin >> x; mf.addNum(x); }
            else cout << mf.findMedian() << "\n";
        }
    }
    return 0;
}
```

三步走"进 lo → 倒给 hi → 不够再补回"，一次性同时保证了**值域有序**和**大小平衡**两个不变量，比分情况讨论清爽得多。约定 `lo.size() >= hi.size()`，奇数个时中位数就是 `lo.top()`。

**215 第 K 大**两种写法：小顶堆 O(N log K)，或快速选择（Quick Select）平均 O(N)：

```cpp
// 快速选择核心：只递归包含第 k 位的那一侧
nth_element(a.begin(), a.begin() + k - 1, a.end(), greater<int>());   // 竞赛可直接用
cout << a[k-1];
```

**347 前 K 个高频**：`unordered_map` 计数后，用小顶堆按频次维护 K 个；或桶排序（下标即频次）做到 O(N)。

---

## 十一、动态规划

### 五大骨架

```
① 线性 DP：       dp[i] 由 dp[i-1] / dp[i-2] 推出            → 70, 198, 53, 152
② 完全背包：      for 物品 { for j = w..W }  正序             → 322, 279
③ 0-1 背包：      for 物品 { for j = W..w }  倒序             → 416
④ 二维串 DP：     dp[i][j] 表示 s1 前 i 个与 s2 前 j 个       → 1143, 72
⑤ 网格 DP：       dp[i][j] = f(dp[i-1][j], dp[i][j-1])       → 62, 64
```

**背包正序倒序的唯一区别**：正序时 `dp[j-w]` 已是本轮更新过的值（同一物品可再选 → 完全背包），倒序时 `dp[j-w]` 还是上一轮的值（每个物品只选一次 → 0-1 背包）。记住这一句，两类背包就分清了。

### 代表题 A：322 零钱兑换（完全背包，求最小个数）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n, amount;
    while (cin >> n >> amount) {
        vector<int> coins(n); for (int &x : coins) cin >> x;
        const int INF = 1e9;
        vector<int> dp(amount + 1, INF);
        dp[0] = 0;                                  // 凑 0 元需要 0 枚
        for (int c : coins)
            for (int j = c; j <= amount; j++)       // 正序 = 硬币可重复使用
                dp[j] = min(dp[j], dp[j - c] + 1);
        cout << (dp[amount] == INF ? -1 : dp[amount]) << "\n";
    }
    return 0;
}
```

求方案数时把 `min(...)+1` 换成 `dp[j] += dp[j-c]`；此时**外层物品/内层容量求的是组合数，内外调换求的是排列数**（377 题的坑）。

### 代表题 B：416 分割等和子集（0-1 背包 + 状态压缩）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n;
    while (cin >> n) {
        vector<int> a(n); int sum = 0;
        for (int &x : a) { cin >> x; sum += x; }
        if (sum & 1) { cout << "false\n"; continue; }     // 奇数直接否
        int W = sum / 2;
        vector<char> dp(W + 1, 0);
        dp[0] = 1;                                        // 容量 0 恒可达
        for (int x : a)
            for (int j = W; j >= x; j--)                  // 倒序 = 每个数只用一次
                dp[j] = dp[j] || dp[j - x];
        cout << (dp[W] ? "true" : "false") << "\n";
    }
    return 0;
}
```

用 `bitset` 还能再快 64 倍：`bs |= bs << x;` 最后看 `bs[W]`。

### 代表题 C：72 编辑距离（二维串 DP 模板，1143 同构）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    string s, t;
    while (cin >> s >> t) {
        int m = s.size(), n = t.size();
        vector<vector<int>> dp(m + 1, vector<int>(n + 1, 0));
        for (int i = 0; i <= m; i++) dp[i][0] = i;      // t 为空：删 i 次
        for (int j = 0; j <= n; j++) dp[0][j] = j;      // s 为空：插 j 次
        for (int i = 1; i <= m; i++)
            for (int j = 1; j <= n; j++) {
                if (s[i-1] == t[j-1]) dp[i][j] = dp[i-1][j-1];       // 免费匹配
                else dp[i][j] = 1 + min({ dp[i-1][j],     // 删除 s[i-1]
                                          dp[i][j-1],     // 插入 t[j-1]
                                          dp[i-1][j-1] }); // 替换
            }
        cout << dp[m][n] << "\n";
    }
    return 0;
}
```

`dp[i][j]` 表示 s 的**前 i 个**与 t 的**前 j 个**，所以字符下标要用 `i-1`、`j-1`，多出的第 0 行 0 列专门放空串边界。**1143 LCS** 只需把转移改成：相等 `dp[i-1][j-1]+1`，不等 `max(dp[i-1][j], dp[i][j-1])`。

### 其余 DP 的一句话状态定义

- **70 爬楼梯 / 198 打家劫舍**：`dp[i] = dp[i-1] + dp[i-2]` / `max(dp[i-1], dp[i-2] + a[i])`，都可压成两个变量。
- **53 最大子数组和**（Kadane）：`cur = max(a[i], cur + a[i]); ans = max(ans, cur);`
- **152 乘积最大**：负负得正，必须同时维护 `mx` 和 `mn`，遇负数交换二者。
- **139 单词拆分**：`dp[i] = 任意 j 使 dp[j] && s[j..i) ∈ dict`。
- **300 LIS 的 O(N log N) 写法**（贪心 + 二分，`tail[i]` 表示长度 i+1 的上升子序列的最小结尾）：

```cpp
vector<int> tail;
for (int x : a) {
    auto it = lower_bound(tail.begin(), tail.end(), x);   // 严格递增用 lower_bound
    if (it == tail.end()) tail.push_back(x);
    else *it = x;
}
cout << tail.size();          // 注意：tail 本身不是任何一个合法的 LIS
```

- **5 最长回文子串**：中心扩散要枚举 2n-1 个中心（奇偶各一套）；`5` / `131` 都可先用 `bool pal[i][j]` 预处理。
- **32 最长有效括号**：栈里存下标、栈底垫一个 `-1` 作基准，`i - st.top()` 即当前有效长度。

---

## 十二、贪心与位运算技巧

### 代表题 A：45 跳跃游戏 II（区间贪心模板，覆盖 55）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n;
    while (cin >> n) {
        vector<int> a(n); for (int &x : a) cin >> x;
        int end = 0, far = 0, step = 0;
        for (int i = 0; i < n - 1; i++) {        // 注意是 n-1：到达最后一格无需再跳
            far = max(far, i + a[i]);            // 本步能覆盖的最远边界
            if (i == end) { end = far; step++; } // 走到当前边界，必须再跳一步
        }
        cout << step << "\n";
    }
    return 0;
}
```

把它理解成 BFS 分层：`end` 是当前层的右边界，`far` 是下一层的右边界，跨越边界即层数加一。**55 跳跃游戏**只需维护 `far`，中途出现 `i > far` 即失败。

**763 划分字母区间**是同一种"边界"思想：

```cpp
int last[26]; for (int i = 0; i < n; i++) last[s[i]-'a'] = i;
int start = 0, end = 0;
for (int i = 0; i < n; i++) {
    end = max(end, last[s[i]-'a']);
    if (i == end) { cout << end - start + 1 << " "; start = i + 1; }
}
```

### 代表题 B：31 下一个排列（四步定式）

```cpp
#include <bits/stdc++.h>
using namespace std;

int main() {
    ios::sync_with_stdio(false); cin.tie(nullptr);
    int n;
    while (cin >> n) {
        vector<int> a(n); for (int &x : a) cin >> x;

        int i = n - 2;
        while (i >= 0 && a[i] >= a[i+1]) i--;            // ① 从右找第一个升序对的左端
        if (i >= 0) {
            int j = n - 1;
            while (a[j] <= a[i]) j--;                    // ② 从右找第一个大于 a[i] 的数
            swap(a[i], a[j]);                            // ③ 交换
        }
        reverse(a.begin() + i + 1, a.end());             // ④ 后缀翻转成最小（原为降序）

        for (int k = 0; k < n; k++) cout << a[k] << " \n"[k+1==n];
    }
    return 0;
}
```

第 ④ 步不能漏，也不能写成排序：`i` 右侧原本必然是非递增的，交换后依然非递增，翻转即得最小后缀，O(1) 完成。`i < 0` 时表示整体降序，翻转后自然回到最小排列。

### 其余技巧题

**136 只出现一次的数字**（异或：`x^x=0`, `x^0=x`）：

```cpp
int ans = 0; for (int x : a) ans ^= x;
```

**169 多数元素**（摩尔投票）：

```cpp
int cand = 0, cnt = 0;
for (int x : a) { if (cnt == 0) cand = x; cnt += (x == cand) ? 1 : -1; }
```

**75 颜色分类**（荷兰国旗，三指针）：

```cpp
int lo = 0, i = 0, hi = n - 1;
while (i <= hi) {
    if (a[i] == 0) swap(a[i++], a[lo++]);
    else if (a[i] == 2) swap(a[i], a[hi--]);   // 换来的值未检查，i 不能动
    else i++;
}
```

**287 寻找重复数**（把 `i -> a[i]` 看成链表，转化为 142 找入环点）：

```cpp
int slow = a[0], fast = a[a[0]];
while (slow != fast) { slow = a[slow]; fast = a[a[fast]]; }
slow = 0;
while (slow != fast) { slow = a[slow]; fast = a[fast]; }
// slow 即重复数
```

**121 买卖股票**：一次遍历维护历史最低价，`ans = max(ans, p - minP)`。

---


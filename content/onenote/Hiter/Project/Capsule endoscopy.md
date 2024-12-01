## 课题已完成工作：

- 阅读文献，查找文献中提及的相关结构方案
    
    1. 两套方案：四杆和杠杆结构（结构复杂，不便于加工）
    2. 四杆机构由于加工精度的限制，导致其运动轨迹不稳定，结构松散（应当在后期方案中减少关节副的使用）
    3. 设计教训：应当尽量简化设计，提高结构的可靠性
    4. 当前paddle/legged 方案的优点是 high velocity，不足是 reverse,stop,damage,retention,==当前需要针对====stop====来改进==，damdge是要在腿部尖端结构上作文章
    5. 三大功能要求：1、前进 2、撑开 3、停留
- 基于已有方案，针对亟待解决的问题进行结构方案设计
- 对结构方案进行动力学仿真（利用ANSYS或者Adams），提高结构可靠性
    
    1. 需要对接触力进行仿真测算
    2. 运动过程分析
    3. 进行刚-柔仿真，测算出接触力的大小
- 对结构进行加工优化
- 设计外壳，使相互之间能够成为一个整体 **已经完成外壳制作
- 利用3D打印外壳，进行结构组装
- 实验验证方案的可靠性
    
    - 做在透明软管中移动的视频
    - 在大空间内胶囊利用外部磁铁进行站立的实验
 
## 论文计划：

- ICIA 第一代机器人
- CBS 活检装置（二作）& 算法创新（三作）
- IROS 二代腿部结构
- 将毛毡贴在胶囊外部，实现对堵塞部分的疏通
 
## 专利：

七个（3个二作，4个三作）

1. 一种基于桨式的主动式腿部伸展与收缩装置的内窥镜机器人
2. 一种基于丝杠的主动式腿部伸展与收缩装置的内窥镜机器人
3. 一种具有腿部伸展与收缩结构的内窥镜机器人
4. 一种具有多方向施药功能的肠道微型胶囊机器人
5. 一种具有多方向活体采样功能的肠道微型胶囊机器人
6. 一种具有施药功能的肠道微型胶囊机器人
7. 一种具有活检功能的肠道微型胶囊机器人

2018104203060 桨式

![专利进展](Exported%20image%2020240403195529-0.png)

2018104203592 受通  
2018104212996 受通  
2018104218901 腿

![发 明 专 利 申 清 公 布 及 进 入 实 质 审 发 明 专 利 申 清 公 布 及 进 入 实 质 审 发 明 专 利 申 清 初 步 审 查 台 格 知 书 用 缍 审 吡 知 书 专 利 申 清 受 理 知 书 2018 一 10 ． 22 2018 一 10-17 2018 一 05 ． 23 2018 一 05 刁 # 2018 一 05 刁 # 深 圳 市 添 源 知 识 产 权 代 理 事 务 深 圳 市 添 源 知 识 产 权 代 理 事 务 518034 518034 518034 518034 518034 2 8D5D7143233 2 8D5D7143233 113 ． gl 20g ． 1 11 113 ． gl 20g ． 1 11 件 发 电 子 发 电 子 发 电 子 发 电 子 发 ](Exported%20image%2020240403195529-1.png)

2018104219016 四杆机构

![发 明 专 利 申 清 公 布 及 进 入 实 质 审 发 明 专 利 申 清 公 布 及 进 入 实 质 审 发 明 专 利 申 清 初 步 审 查 台 格 知 书 用 缍 审 吡 知 书 专 利 申 清 受 理 知 书 2D18 刁 g 一 11 2018 一 09 刁 5 2018 一 05 ． 23 2018 一 05 刁 # 2018 一 05 刁 # 深 圳 市 添 源 知 识 产 权 代 理 事 务 深 圳 市 添 源 知 识 产 权 代 理 事 务 518034 518034 518034 518034 518034 2 8D5D7143232 2 8D5D7143233 113 ． gl 20g ． 1 11 113 ． gl 20g ． 111 件 发 电 子 发 电 子 发 电 子 发 电 子 发 ](Exported%20image%2020240403195529-2.png)

2018206602323 实用  
201820660222X 实用
 
## 比赛：

- ICRA DJI RoboMaster AI Challeng 第二名
- 京东无人车挑战赛 第三名
 矛盾点：当前能够实现停滞功能的只有仿虫的的结构形式，我的设计方案只能实现胶囊机器人的站立，并非停滞  
解决思路：

- 实现前进和撑开，实现机器人在大空间内能够站立（例如在胃部能够进行施药采样），位姿的切换不用考虑，二者是相互独立的。
- 基于leg-locomotion的设计方案，添加直立功能（现在拟定直立功能的状态是前进状态的一个极限状态）  
前期工作是基于混合动力进行的结构设计，后期的结构需要脱离外部驱动，实现完全的内部驱动（永磁体用来改变空间位姿）
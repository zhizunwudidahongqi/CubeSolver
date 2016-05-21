# 魔方求解器
## 2015程序设计基础大作业
##### 输入输出
使用标准输入输出
##### 输入格式
依次输入6个面的颜色信息，颜色用首字母BRYGOW表示，面顺序为FBLRUD。
每个面可用3\*3或1\*9输入，面内顺序为从左上角开始水平扫描。
看每个面的视角规定为将表面以F为中心展开。
（输入顺序和内部编码顺序**不一致**）

	             ┌---┬---┬---┐
	             | 36| 37| 38|
	             ├---┼---┼---┤
	             | 39| U | 41|
	             ├---┼---┼---┤
	             | 42| 43| 44|
	             └---┴---┴---┘
	┌---┬---┬---┐┌---┬---┬---┐┌---┬---┬---┐┌---┬---┬---┐
	| 18| 19| 20|| 00| 01| 02|| 27| 28| 29|| 09| 10| 11|
	├---┼---┼---┤├---┼---┼---┤├---┼---┼---┤├---┼---┼---┤
	| 21| L | 23|| 03| F | 05|| 30| R | 32|| 12| B | 14|
	├---┼---┼---┤├---┼---┼---┤├---┼---┼---┤├---┼---┼---┤
	| 24| 25| 26|| 06| 07| 08|| 33| 34| 35|| 15| 16| 17|
	└---┴---┴---┘└---┴---┴---┘└---┴---┴---┘└---┴---┴---┘
	             ┌---┬---┬---┐
	             | 45| 46| 47|
	             ├---┼---┼---┤
	             | 48| D | 50|
	             ├---┼---┼---┤
	             | 51| 52| 53|
	             └---┴---┴---┘  序号为输入顺序

##### 输出格式
* 第一部分：
输出读入的魔方状态，用数字表示颜色（BRYGOW => 012345）
* 第二部分：
输出通俗表示的复原步骤，每行代表一组操作。
* 第三部分：
输出规定格式的复原步骤，仅含12种单步操作，每个一行。
##### 算法原理
模拟CFOP，在复原完顶层十字后，进行随机化处理。




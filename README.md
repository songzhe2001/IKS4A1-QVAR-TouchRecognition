# STM32-IKS4A1的QVAR触摸识别

## 识别原理及流程 

1、使用迟滞思想，将QVAR的输入量化为1，0，-1。 

2、对量化后的数据进行延时去抖 

3、将近三次数据进行分类 

## 使用方法 

1、传入qvar的测量数据，类型为int16_t，单位为mv的请将输入数据×78。

2、给定输出的变量，类型为int *。

3、本人测量数据频率约为1Khz，其他频率请自行更改去抖参数。 

## 结果说明 

4、-4为双击，2、-2为点按，1、-1为滑动，0无操作。 




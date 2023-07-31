# Stock-Investment-Strategy
基于动量因子选择股票并进行行业回测，数据基于中信全指和中信一级行业。

算法核心思路：
1. 寻找信号触发日。（满足下跌超过阈值D,回弹不超过阈值U,触底反弹超过阈值U）
   ![3](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/1ad7a128-0348-4e13-b32f-2ba970ad154a)

   计算结果如下：
   
   ![statistic_day_0](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/8ce5fee2-7409-4243-a427-f4e6796cabf4)
   ![statistic_day](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/f5403466-8a64-4546-86fc-3dc7808153b2)


   
3. D和U根据市场的波动程度进行动态调整。
![2](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/1938e341-444a-4615-889f-c8272a0a3d1c)

   计算结果如下：
   
![ATR](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/ce1c4668-a6f1-4abf-9ccc-9d199d4e3a47)
![DU](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/bcca10ef-fd61-475a-a43c-3e13bc653114)


   
5. 计算信号日当天各股的反弹动量。
![1](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/fb954e68-244e-4333-8d71-73430516b003)

   
6. 根据反弹动量数值关系完成投资。
![4](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/125389f7-6560-4c0d-be1c-0eab0f8a5340)

   计算结果如下：
   
![earned_money](https://github.com/ArcherCYM/Stock-Investment-Strategy/assets/49087999/6958b061-ca24-4805-91f2-83ee7cc6aab3)

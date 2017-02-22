# 期货策略01

高低点策略
reference:  <爱建证券_20160405_量化策略研究之一：基于高低点突破，高低点反转，头肩顶反转的研究>


key:最原始的高低点突破，不做任何过滤，只要突破上一个高点就做多，突破上一个低点就做空。
既然是高低点突破首先要定义高低点，然后就是当股价S上穿定义好的前高点后做多，下穿前低做空。而高低点的定义我们可以使用左右臂的方式去定义它，即，一个高点形成前的上涨阶段(左臂)，以及此后下跌后的下跌阶段(右臂)。如果K线最高价不断提高，那么左臂数加1，右臂数始终为0，直到股价连续下跌，跌出足够多的右臂累加数量后，我们认为前高已形成。以上为前高低点的定义。同样的，当前高低点定义好后，我们只需要静静等待一个突破的过程。
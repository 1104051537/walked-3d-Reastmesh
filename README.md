# 一种直接从可行走的场景模型生成导航网格的方案

众所周知，游戏内导航网格的生成一般使用RecastNavigation。其中有几个步骤，大致为：1 模型体素化 2过滤出可行走表面 3生成region（三维分割为二维） 4生成边缘 5生成凸多边形 6生成细致的三角导航网格，但是对于只有可行走表面的场景模型，就没必要经过1和2这两步，我们只需要

# 关卡配置信息

详细信息参考 LevelTemp.txt 文件  
>通用字段说明：
  
	"idx":0,               道具索引第一个为0，后面依次增加
    "type":"BoxWater",     道具类型
    目前支持的道具：
  	1.BoxWater(开关)
  	2.BoxFire(煤气灶)
  	3.BoxTemp(温度计)
  	4.BoxTea(热水壶)
  	5.BoxCircle(风扇)
 
    "position":[-280,100],  道具位置坐标
    "rotation":0,           道具旋转角度//暂时不用动
    "scale":[0.3,0.3],      道具缩放大小
    
>boxInfo字段说明    
   
    "boxInfo":{             配置道具条件相关属性 
        "value":2,           目标时间（秒）
        "isClockCicle":false,顺时针或逆时针转动  
        "maxWrongValue":0.5, 最大容错值
        "startType":"preBoxDelay",  触发条件
        1.normal 立即启动
        2.delay 延时启动
        3.preBoxDelay  前置道具条件成立启动
        
        "isAutoFail":true,  是否开启时间到，自动失败
        "preBoxIdx":1,  前置道具索引号
        "startDelayTime":1,  延时（秒）开启，仅对 delay  preBoxDelay类型有效
        "totalAutoFailTime":2  道具激活后，自动等待（秒）后失败
    
    
>boxInfo信息根据不同的道具会有差异    
详细参考json文件和LevelTemp.txt文件
  


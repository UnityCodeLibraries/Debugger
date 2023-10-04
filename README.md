# Debugger
一个用于Unity运行时的UI面板展示一些控制台信息

# S2.0

### 应用场景: 
- 当你可能要在不同测试阶段查看不同的测试信息并需要动态筛选时可以使用此组件
### 如何使用: 
#### 配置
1. 添加一个Gameobject并挂载RuntimeConsole组件
1. 创建ShowTags预设并挂到该组件上
1. 将你想要显示的标签添加在预设列表
#### 使用与查看
1. 然后你就可以使用MyDB.DL/LW来输出日志信息并在Console或游戏中实时查看
```
  MyDB.DebugCallback = true;//开启输出回调
  
  MyDB.DL("V1", "这是一条Log信息");
  MyDB.LW("V1", "这是一条Warn信息");
  MyDB.LW("V2", "按~键切换显示游戏调试信息台");
  MyDB.DL("V3", "这是一条不会显示的Log信息");
  MyDB.LW("V2", "Collapse切换集中显示, ScrollBottom切换自动滑底");
  MyDB.DL("V2", "kkk\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\n\nkkk");
```
#### 更新标签
1. 可以随时通过增加或移除ShowTags预设来过滤你需要的标签
1. 或者直接拖入不同的预设来更改过滤配置
#### 实时控制台
1. 按~键切换显示游戏调试信息台  
    - Collapse切换集中显示, 
    - ScrollBottom切换自动滑底  
### 更新信息: 
将绑死的ShowTags优化为ShowTagsPreset预设

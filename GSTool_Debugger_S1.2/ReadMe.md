# S1.2

### 应用场景: 
- 当你可能要在不同测试阶段查看不同的测试信息并需要动态筛选时可以使用此组件
### 如何使用: 
1. 添加一个Gameobject并挂载RuntimeConsole组件
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
3. 可以通过增加或移除ShowTags来过滤你需要的标签
1. 按~键切换显示游戏调试信息台  
1. Collapse切换集中显示, ScrollBottom切换自动滑底  
### 更新信息: 
更新了命名空间改为gstools
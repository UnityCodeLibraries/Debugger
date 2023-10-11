# Debugger
一个用于Unity运行时的UI面板展示一些控制台信息

# GsTool_Debugger_V2.4.0.231011.alpha

### 应用场景: 
- 当你可能要在不同测试阶段查看不同的测试信息并需要动态筛选时可以使用此组件
### 现有功能: 
#### 新的: SingleLoggerWindow
##### 配置
1. 从Prefabs将SingleLoggerWindow预制件拖入场景中即可
##### 更新配置
1. 修改示例标签: 
    - 修改Presets下示例预设的ShowTags列表即可
1. 启用或禁用: 
    - tag后加Ban即为禁用
    - 反之启用
1. 增加预设: 
    - Project窗口右键Create直接创建ShowTagsPreset并挂载到SingleLoggerWindow组件上即可
##### 使用
- 直接调用Unity log方法即可, 格式为tag加:号加yourMes, (需要ShowTagsPreset存在此tag)
```
      Debug.Log("Tag: 显示的消息");
```
##### 旧版: 实时控制台
1. 启用: 
    - 挂载RuntimeConsole组件即可启用, (已过时)
1. 使用: 
    - 按~键切换显示游戏调试信息台  
        - Collapse切换集中显示, 
        - ScrollBottom切换自动滑底  
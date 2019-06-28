![Editor](../../../Images/Component/TimeInfoExecuteComponent.png)

在1.0.9版本之前事件是在模块编辑器中进行添加,所有的时间点都需要进行添加,同时也会修改AnimationClip的meta文件,如果项目没有同步meta文件,那么运行时将会没有任何反应,所以在1.0.9以后是在运行时进行添加,在1.1.0版本之前这段逻辑是在`AnimationClipInfoAssetManagerComponent`组件中进行添加,1.1.0改为在`TimeInfoExecuteComponent`组件进行添加,同时也更符合设计,因为它不是必须的


对于1.0.9版本之前的使用者,想删除以添加的动画事件,可以选中动画右键`Icarus/IcAnimation/RemoveAll ACITExecute Animation Event`来进行删除,支持多选

![Editor](../../../Images/Component/removeACITExecuteEvent.png)
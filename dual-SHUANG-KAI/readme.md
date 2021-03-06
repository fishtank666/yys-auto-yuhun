## 阴阳师本地双开脚本 

请首先参考上一级的 [README.MD](../README.md)，并确认您理解一切内容！ 

### 使用方法 

本地双开阴阳师桌面版模拟器，登录你的大号小号。
窗口可以被遮挡，但是不能最小化。
作者使用了 V5 模拟器进行测试 (This is NOT an endorsement)。

__Python 脚本和游戏窗口都必须以管理员权限运行！__

小号（司机）点击 组队-选择你要打的副本-不公开-邀请大号-大号点击绿勾确认。
此时你的大号小号应该都进入了“协战队伍”的列表。

大号小号都 __需要__ 锁定阵容。

挂机界面请参考 ![](zudui.png)如果 YYS 游戏的 UI 更新了，你看到的游戏御魂准备界面不是这样的，你可以自行修改“挑战”按钮对应的坐标和颜色，或者发 Issue 等待开发者不定期更新。

运行 Python 脚本。
脚本默认点*右边*的怪， 如需点中间或者不点怪，请手动修改第24行 `emyc` 的值。 
(如果有兴趣你可以发PR，把这里换成弹窗或者 terminal 输入。)

在战斗中请勿旋转镜头或者移动小号的窗口，可能会出现视角乱转。

随时使用 Ctrl+C，或者任务管理器中断脚本。 
(如果有兴趣你可以发PR，添加 keyboard capture.)

### 可能存在的问题 

* （应该）可以自动拒绝悬赏。
* 脚本可以在每一轮结束后自动邀请队友，战斗成功或失败都可以。
* ~~作者使用的是新号自带的默认庭院皮肤“初语谧景”进行测试。
如果你使用了其他的庭院皮肤，由于在结算过程中可能点到召唤灯笼或其他界面UI，
作者暂时无法保证这里不会出错。
如果发现存在乱点“邀请”或者“进入召唤灯笼”的情况，请发 Issue，并附上最后几行的程序输出。~~
感谢 [#5](https://github.com/society765/yys-auto-yuhun/issues/5) 提出的意见，战斗结算的点击区域已修改。
* 不能处理体力不足，或者御魂数量过多的提示框。
* 当上一次战斗失败后，小号会自动继续邀请大号。这时存在极微小的概率，
大号点绿勾（战斗失败不能点自动接受邀请）上了别人的车。这个我也无能为力。
* [#6](https://github.com/society765/yys-auto-yuhun/issues/6) 提出使用双开脚本有警告的风险，作者本人尝试了双开100体力暂时没遇到问题。 
__使用该脚本风险自负，责任与作者无关。USE AT YOUR OWN RISK!__
* 其他？请发 Issue.

### 其他 

作者2018年肝面灵气绘卷之后弃坑了，这个双开脚本最初是作者在按键精灵里使用过的，
用 Python 简单重写了一下后传了上来，可能在重写时存在些许 bug。
感谢您的测试及反馈。


该源代码使用了 [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) 开源协议。  
This project is licensed under the [GPLv3](https://www.gnu.org/licenses/gpl-3.0.html) license.


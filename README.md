# Ocean Muck · 深蓝漂流

原创低多边形斜俯视角海洋生存游戏，使用 Three.js 和原生 JavaScript。

## 游玩

GitHub Pages 启用后：https://wuhuyixia.github.io/Ocean-Muck/

在仓库 Settings → Pages → Build and deployment → Source 选择 Deploy from a branch，选择 main / (root)，点击 Save。无需构建。

本地测试：在仓库根目录执行 `python -m http.server 8000`，访问 http://localhost:8000/ 。首次加载需要访问 jsDelivr CDN 获取 Three.js 0.160.0。

## 操作

- WASD / 方向键移动，鼠标滚轮缩放；触屏提供方向按钮。
- 1 打捞钩，点击投掷；2 地板，3 收集网，4 武器，5 净水器，6 捕鱼器，7 工作台。
- E 采集，F 吃鱼，R 喝水，B 制作/升级，空格攻击，Esc 暂停。
- 白天打捞与登陆岛屿，夜间海怪袭击。设备每 8 秒生产资源，宝箱提供随机强化。

## 存档

每 15 秒自动保存到 localStorage，切换页面/暂停时也保存；支持手动存档与 JSON 导入导出。每浏览器一份存档，新建或导入会覆盖旧存档（需确认）。死亡结束本局。存档保存人物、资源、世界种子、木筏、设备、等级和生存时间；动态敌人、漂浮物、采集冷却在重新加载后重置。无云端同步。

## 当前版本

v0.1 原型：有限范围的程序化海域、14 座岛屿、资源采集、打捞、建造、昼夜、战斗与随机强化。没有多人模式、完整物理模拟或 Boss。

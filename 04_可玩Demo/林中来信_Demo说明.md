# 林中来信 · Demo v0.2

Windows 单人第一人称原型。新版实现从前情提要到结局的完整流程，增加扫描、构造、稳定设备和小红帽同行演出。

运行 ../build/LittleRedDemo/LittleRed.exe，免安装、离线运行。完整操作见 PLAY.txt，逐段流程见 docs/DESIGN.md。

Q 切换设备与空手/武器，滚轮选择功能，按住左键使用；E 调查、对话，WASD 移动，Shift 快走，Tab 笔记，F 手电，Esc 暂停。最终战可射击、R 换弹，G 启动一次短暂强化。

新游戏播放三段前情提要，E 继续，长按空格跳过。检查点保存调查、桥梁修复及通路状态；读档不重播前情。新版存档 little_red_v02_checkpoint.json 位于 %APPDATA%/Godot/app_userdata/Project X · 林中来信/。旧存档保留，不兼容新版路线。

场景、设备、人物由程序几何生成；有中文字体和原创合成声音，无配音或精细骨骼动画。15–20 分钟为目标，尚未真人计时。具体台词、关卡机关和结尾通讯是 Demo 实现稿，不自动成为系列正式设定。

Godot 4.7.2 标准版打开 project.godot。执行 ./build.ps1 -Test 可导入、检查前情与整章流程、导出 Windows 版。chapter.gd 管理设备与新增剧情，chapter_world.gd 管理机关几何；main.gd 管理主流程、战斗、界面与存档。tests/ 为独立测试，发行版不包含测试及截图。

验证记录见 docs/VERIFICATION.md。字体和 Godot 许可证随包提供。GitHub 尚未上传，待提供目标仓库。

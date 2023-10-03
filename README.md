<div align="center">
  <a href="#"><img src="https://kiramibot.dev/img/logo.svg" width="180" height="180" alt="KiramiBotPluginLogo"></a>
</div>

<div align="center">

# kirami-plugin-horserace

_✨ 群内赛马小游戏 ✨_


<a href="./LICENSE">
    <img src="https://img.shields.io/github/license/FrostN0v0/kirami-plugin-horserace.svg" alt="license">
</a>
<a href="https://pypi.python.org/pypi/kiramibot-plugin-example">
    <img src="https://img.shields.io/pypi/v/kirami-plugin-horserace.svg" alt="pypi">
</a>
<img src="https://img.shields.io/badge/python-3.10+-blue.svg" alt="python">

</div>

## 📖 介绍

适用于KiramiBot的赛马小游戏插件

由 [zhenxun_bot_HorseRace](https://github.com/Evan8440/zhenxun_bot_HorseRace) & [nonebot_plugin_horserace](https://github.com/shinianj/nonebot_plugin_horserace) 适配而来,稍作修改，添加合并消息返回配置项

## 💿 安装

在 KiramiBot 项目的插件目录下, 打开命令行, 根据你使用的包管理器, 输入相应的安装命令

<details>
<summary>pip</summary>
  
```bash
pip install kirami-plugin-horserace
```
</details>
<details>
<summary>pdm</summary>

```bash
pdm add kirami-plugin-horserace
```
</details>
<details>
<summary>poetry</summary>

```bash
poetry add kirami-plugin-horserace
```
</details>
<details>
<summary>conda</summary>

```bash
conda install kirami-plugin-horserace
```
</details>

打开 KiramiBot 项目根目录下的配置文件, 以 `kirami.toml` 为例，在 `[plugin]` 部分追加写入
```toml
plugins = ["kiramit_plugin_horserace"]
```

## ⚙️ 配置

在 KiramiBot 项目的配置文件中添加下表中的必填配置

| 配置项 | 必填 | 默认值 | 说明 |
|:-----:|:----:|:----:|:----:|
| send_forward_msg | 否 | True | 将图片以合并消息发送 |
| pic_font_size | 否 | 16 | 图片字体大小 |
| setting_track_length | 否 | 20 | 跑道长度 |
| setting_random_min_length | 否 | 0 | 随机位置事件，最小能到的跑道距离 |
| setting_random_max_length | 否 | 15 | 随机位置事件，最大能到的跑道距离 |
| base_move_min | 否 | 1 | 每回合基础移动力最小值 |
| base_move_max | 否 | 3 | 每回合基础移动力最大值 |
| max_player | 否 | 8 | 最大支持玩家数 |
| min_player | 否 | 2 | 最小支持玩家数 |
| setting_over_time | 否 | 120 | 超时允许重置最少时间，秒 |
| event_rate | 否 | 450 | 事件概率 = event_rate / 1000 |

## 🎉 使用
### 指令表
| 指令 | 权限 | 需要@ | 范围 | 说明 |
|:-----:|:----:|:----:|:----:|:----:|
| 赛马创建 | 群员 | 否 | 群聊 | 创建游戏 |
| 赛马加入 [你的马儿名称] | 群员 | 否 | 群聊 | 加入赛马游戏 |
| 赛马开始 | 群员 | 否 | 群聊 | 开始游戏 |
| 赛马重置 | 主人 | 否 | 群聊 | 重置已有赛马 |
| 赛马清空 | 主人 | 否 | 群聊 | 清空已有赛马 |
| 赛马事件重载 | 主人 | 否 | 群聊 | 重载事件文件 |

### 效果图

<img align="left" src="https://ghproxy.com/https://raw.githubusercontent.com/FrostN0v0/kirami-plugin-horserace/master/example1.jpg" width='380px' alt="示例1">

<img align="left" src="https://ghproxy.com/https://raw.githubusercontent.com/FrostN0v0/kirami-plugin-horserace/master/example2.jpg" width='380px' alt="示例2">
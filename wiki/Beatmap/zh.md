---
tags:
  - mapset
  - beatmapset
---

# 谱面

**谱面**（Beatmap，有时称作*Beatmapset*）是一组多个游玩级别（[难度](/wiki/Beatmap/Difficulty)），由各种[击打物件](/wiki/Hit_object)组成，通常代表一首歌曲。它还包括其他成分，所有这些成分都打包在一个带有[“.osz”扩展名](/wiki/Client/File_formats/Osz_(file_format))的文件中：

- 歌曲本身，以mp3或ogg格式存储。
- [背景图片](/wiki/Beatmap/Background)或视频填充游戏区域。
- [自定义击打音效](/wiki/Beatmapping/Hitsound)用于排列和改进听觉反馈（可选）。
- [故事板](/wiki/Storyboard)带有运动图形与特效，用于背景故事和主题（可选）。
- [自定义皮肤](/wiki/Skinning)用于改变界面和游戏元素的外观（可选）。

*注意：谱面的一些视觉和听觉功能可以通过[视觉设置](/wiki/Client/Interface/Visual_settings)禁用。*

## 难度

*请参阅：[难度](/wiki/Beatmap/Difficulty)*

一个难度是一个带有[“.osu”扩展名](/wiki/Client/File_formats/Osu_(file_format))的文件，带有击打物件，击打音效以及如[Kiai 时段](/wiki/Gameplay/Kiai_time)的特效。它还包括[难度设置](/wiki/Client/Beatmap_editor/Song_Setup#difficulty)以及其他直接影响游戏性的参数。谱面的每个难度都有不同的结构，有时只能在一种[游戏模式](/wiki/Game_mode)上游玩。 [星级](/wiki/Beatmapping/Star_rating)评定系统用于可视化这个难度的技能要求。

## 提交谱面

*请参阅：[提交谱面](/wiki/Submission)*

谱面作者可以将自己的创作提交到[谱面列表](https://osu.ppy.sh/beatmapsets)。虽然每个谱面都是一个人做的，但通常视为一个共同的成果：一些难度可能是其他[合作](/wiki/Beatmap/Beatmap_collaborations)或[单个人](/wiki/Beatmap/Guest_difficulty)做的。

提交后, 谱面会得到额外的元数据，比如简介，语言，种类以及明确的内容标记，谱面作者可在网页上自行更改这些字段。 谱面还会获取[标题文本](/wiki/Beatmap/Title_text)，其外观可能会在[谱面提名团队（BN）](/wiki/People/The_Team/Nomination_Assessment_Team)的帮助下进行更改。

### 标识

每个提交的谱面集都被分配了一个数字标识符（`BeatmapSetID`），通过它可以在网站上和通过[osu！api]（/wiki/osu！api）进行跟踪。单个谱面也有自己的数字标识符（`BeatmapID`）。谱面页上指向特定难度标签的URL包含两个标识符，格式如下：
```
https://osu.ppy.sh/beatmapsets/{BeatmapSetID}#{GameMode}/{BeatmapID}
```

## 谱面类别

*请参阅: [谱面类别](Category)*

被提交到网站上的谱面会依照其最近活动情况、提名状态、及流行度被分入不同的谱面类别中：

- [Graveyard](Category#graveyard)
- [Work in Progress / Pending](Category#work-in-progress-and-pending)
- [Qualified](Category#qualified)
- [Ranked](Category#ranked)
- [Approved](Category#approved)
- [Loved](Category#loved)

有些类别有[Ranking准则](/wiki/Ranking_Criteria)，使谱面能够获得暂时或永久的[排行榜](#leaderboards)。实现这一点最常用的方法是[让谱面进入Rank序列使其变为Rank](/wiki/Beatmap_ranking_procedure)，另一种是让谱面变为[Loved](Category#loved)。

## 下载谱面

可以通过一些不同的途径来获取谱面：

### 谱面列表

网站上的[谱面列表](https://osu.ppy.sh/beatmapsets)提供了各种类别的谱面。你可以根据特定条件进行筛选（例如一些谱面创作者创建的[osu!taiko](/wiki/Game_mode/osu!taiko)的谱面），然后逐个下载。[osu!支持者](/wiki/osu!supporter)可以使用更完整的筛选器，比如能够看到他们获得某个等级的谱面。

### osu!direct

osu!direct是内置在游戏客户端内的谱面列表，用于快速访问并供应与网站上列表相似的功能。此功能仅[osu!支持者](/wiki/osu!supporter)可用。

### 非官方信息

除了上面还有谱面的二级来源，osu团队既不检查也不操作这些来源！然而他们可以在论坛上看到，并受到社区的赞赏。这些来源包括：

- 平台外托管的第三方谱面镜像；
- 玩家制作包并通过p2p网络汇编共享，比如BitTorrent。

## 谱面与社区

### 排行榜

osu!中所有玩家都通过谱面与在[全球排行榜](/wiki/Performance_points)中的其他玩家[相互竞争](/wiki/Ranking)。 osu!有不同类型的谱面特定排行榜，除第一个以外，所有都仅对osu!支持者可见：

- 全球排名，适用于活跃的玩家群；
- 每种[游戏模组](/wiki/Game_modifier)的全球排名；
- 由同一张国旗旗组成的特定国家排名；
- 玩家在地图上相对于其好友的位置的好友排名。

谱面中每个难度的前500位都提供了[回放](/wiki/Gameplay/Replay)，可以在线观看，也可以保存下来，以便在本地排行榜上进一步展示。

### 图表和聚光灯

*请参阅：[聚光灯](/wiki/Beatmap_Spotlights)*

自成立之初，该社区就以各种方式展示独特优秀的图。最早记录在案的办法法之一是月度与季节图表，其中包含了排名靠前的beatmaps的一小部分，排行榜上显示地图总分的顶级玩家将获得[osu!支持者标签](/wiki/osu!supporter)。
图表系统后来形成了[聚光灯项目](/wiki/Beatmap_Spotlights)，目前在类似的条件下运行，但改为在osu!lazer的播放列表中运行

### 谱面竞赛

*请参阅：[竞赛](/wiki/Contests)*

osu!社区中定期举办不同的竞赛，以促进创造力，并奖励尽力而为的麻婆。比赛范围从在当地社区内举办的小型比赛，到在全球范围内举办的、有大奖的大型比赛。获奖者通常会获得[osu!支持者标签](/wiki/osu!supporter)和个人简介徽章。

### 精选艺术家

*请参阅：[精选艺术家](/wiki/Featured_Artists)*

精选艺术家是[osu!团队](/wiki/People/The_Team)的一个社区项目，重在授权不同艺术家为osu!创作音乐并使其可用与作图。该网站的[精选艺术家列表](https://osu.ppy.sh/beatmaps/artists)展示每一位参与的艺术家，并提供用于作图的预制模板。

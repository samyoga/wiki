# 世界经济规则

这里包含喵窝世界的经济设定与规则。为保持简洁，相关的命令可能不会详细说明用法。请查阅对应插件的 Wiki 专页或论坛相关帖子了解具体的使用方法。


------

## 基本设定

1. 喵窝世界实行**自由市场经济**。物品价格由市场（玩家）决定。
1. 系统会通过命令、或借助管理员提供交易、传送等服务，其中一部分收费、或加收税费，收费标准基本保持稳定。  
如管理组需要调整税率或修改系统服务价格，将会提前通知。
1. 世界内流通货币单位为**「节操」（简称“节”）**。
  * 每位玩家在首次进入服务器时将**赠送 450 节操**用于购买基础物品。
1. 世界内设置一个公共账户，称**「系统余额」（又称「系统 balance」）**。
1. 一切交易过程中的“征收”“加收税费”，以及系统服务收费（[玩家提供的](#玩家提供的系统服务)除外），均流入「系统余额」。
部分种类的[在线奖励](#在线奖励)，分发时从「系统余额」划扣。
1. 喵窝世界中允许多种交易模式。但有一点是共同的：**商品一经售出，原则上不接受退换（插件不支持）。具体退换货条例请以商家说明/协商结果为准。没有明确说明的，请以不支持退换为准。**
1. 玩家被允许**负债**（即现金额为负数）。负债状态下，玩家仍可使用收费命令，但部分需征税的经济服务将会受限（如木牌交易）。
  * 「系统余额」同样被允许“负债”。这种情况多发生于通过红包道具、回购等服务，从「系统余额」支取过度。此时，系统将启动应急机制，以尽快回笼节操（例如自动拍卖、止付部分签到奖励）。

以下将允许的交易模式以及对应的要求、费用等列出。

## 交易细则

?> :information_source: 关于如何使用交易功能，见 [经济插件使用指南](space/plugins/hamsterecohelper.md)。

### 交易物品限制

!> **注意！天下没有完全自由的市场。**为确保新玩家获得完整的游戏体验，一些针对*Infinite Infernal* （无尽地狱，以下简称 Inf）世界的道具被限制出售。  
对于 Inf 道具的定义，见 [Inf 装备道具图鉴](inf/items.md)。  

?> :heavy_check_mark: **其余未标明的道具不受影响，可正常流通。**

- <span style="color: red">以下 Inf 道具类型的流通受到管制：</span>
  * **矿物块、天界魔矿；**
  * **防具、武器；**
  * **Boss 相关的召唤物、奖励材料、武器和防具。**
- 不允许向其他玩家**越级**直接出售以上道具。  
  + **越级**指出售的物品超出买家已有 Inf 道具的最高档次，或超出买家当前获取该档次物品的能力。
- 不允许在部分位置公开出售 **绿色稀有度（T3）及以上** 的上述管制道具。其中包括：
  + 上架至天喵商店；
  + 在月耀城商店放置 NPC 并出售。
- 对于以上物品，依旧可以进行广告宣传，并在**其它位置**出售（木牌商店、当面交易、天喵直送等），但仍不允许越级出售。
- 可向其他玩家**暂时**越级租借防具或武器，供其体验。**但体验期不得超过 30 分钟。**
- 管理员将不定期对市场进行检查清理，天喵商城的物品**会以回购价格征收**，月耀城的 NPC **会被清理**。


- 此外，**不欢迎**新玩家通过商店，直接购买高级装备和武器。

### 天喵木牌商店

- 用于公共交易的木牌，必须设置在店面中。除明文允许外，不可以设置在其他位置。（其他可能的位置：自己家中用于管理商店。）
- 店面原则上必须设置在各城镇村落中的商业区，城镇规划有另行规定的，按照具体规定执行；EpicWorld 不做限制，为方便玩家使用，建议设置在安全的方位；其他世界不允许设置玩家商店。
- 玩家允许自由入驻商业区中的空店面（部分地区的店面需购买）。占用店面请立即装修并设置商店。如果因为各种原因不能立即开始使用，需要贴牌占用。占用说明木牌必须在店面入口明显处并标明占用者 ID。不符合要求或过期的占用木牌视为无效。
- 店面必须保持活跃。如果一个商业街中出现了不活跃的店面（没有有效木牌或商品，且负责玩家最后上线在 30 天前），其他需要使用店面的玩家可以申请拆除该店面。


- 玩家可以创建 8 个木牌。
  + 木牌可以是“SELL”（出售）、“BUY”（收购）、或“LOTTO”（抽奖）。
- 玩家的出售区可以使用 128 个物品槽。
- 每次交易加收 2% 消费税。
- 所有的 Lotto 木牌必须在木牌描述或附近的木牌上注明抽奖内容物品和奖率。如实写明的 Lotto 木牌交易由使用者（交易发起者）自行承担。

### 天喵商城

- 天喵商城（`/hm`）允许玩家随时随地上架、浏览、购买物品。
- 玩家允许上架最多 **12 个槽**的物品。
- 每次上架均征收 **39 节操**手续费。
- 商城中上架的物品如未售出，每个槽每日会征收 1 节操的保存费用。
- 每笔交易加收 8% 消费税。

### 征购与拍卖

- **基于征购和拍卖的特性，所有交易均为最终交易，不可变更。**
- 每次拍卖成交后，成交额的 10% 将被征收。


- 当「系统余额」陷入负值，系统将开始自动拍卖随机物品，直至回笼足够节操为止。
  + **注意：**这些物品不一定适用于当前版本。

### 一对一账单交易

- 每份账单结算时，加收 2% 消费税。

## 系统服务收费细则

### 即时传送

玩家可使用系统服务提供的传送命令让游戏更加便利。但是这些命令价格较高，建议首选其他玩家提供的铁道、空港/飞行塔或传送牌。

- `/spawn` 和 `/espawn` 暂定免费。
- `/home` 和 `/back` 根据距离计算价格，所有的费用均保存到系统 balance。计费策略：
  - 起步价均为 **9 节操**；
  - 距离以玩家当前位置开始计算（跨世界额外加 9 节操，距离以目标所在世界的出生点开始计算）；
  - 距离每增加 100 米，加收 1 节操；
  - 每次传送收费最高 198 节操。
- `/sethome` 根据距离计算价格，所有的费用均保存到系统 balance。计费策略：
  - 起步价 **450 节操**，主世界以外加收 42 节操；
  - 距离以当前世界出生点开始计算，每增加 100 米，减免 20 节操（即距离出生点越远越价格越低）；
  - 最低可降至 45 节操。
- 修改出生点/村落间传送 `/town select` **每次 45 节操**。这将影响你的 `/spawn` 目标点。新玩家第一次设置免费。
- 传送牌每次传送费用由所有者于牌上标明。

其中，`/spawn` 前往的出生点为玩家 [选定的出生点](nyaa/realms) 或默认的世界出生点，`/espawn` 前往的出生点始终为默认的世界出生点。

### 领域规划

玩家可为自己所管理的村落或规划区建立领域提示。建立提示后，将展示规划区名称和管理玩家。

领域规划必须由管理组审核后操作。**对于玩家村落免费**，特殊规划提示价格为每个方块 1 节操。（占地面积 x 高度，一般 256）

### 邮送物品

邮送物品支持单手物品（一个或多个堆叠），或一次发送一个箱子的物品。服务价格如下。

- 1.0 节操单手物品包邮
- 39 节操一箱物品包邮

### 广告服务

**该服务用户体验不佳，目前已关闭。可借助天喵商城发布广告。**

> 玩家可以使用广告服务提升销量或达到其他非恶意宣传的目的。广告会在聊天区域中轮播，频率是 2 分钟一条。允许使用大部分样式代码，允许的最大文本长度是 140 个字符。
>
> 当前广告的费用是 1 节操/次展示，发布广告最低 10 最高 400 次展示。
>
> 展示的计算策略是 `在线玩家 - (广告主 + AFK 玩家)`。
>

### 重命名

#### 前缀/后缀/昵称

玩家可自助更改在喵窝世界之昵称，以及昵称的前、后缀。请注意不要使用令人反感的词句或冒充他人。

- 更改前缀：42 节操 + 100 exp/次 `/nu prefix [前缀]`
- 更改后缀：42 节操 + 100 exp/次 `/nu suffix [后缀]`
- 自定义昵称：免费。`/nick [自定义昵称]`

例如 `/nu prefix &a我&b是&c前&d缀`

如要重置前/后缀，请使用 `/nu resetprefix` 和 `/nu resetsuffix`。这些命令不收取费用。
自定义昵称不影响实际游戏 ID。

#### 物品重命名

使用 `/nu rename [名称]` 可以重命名手中的物品，价格为 45 节操 / 个。
请注意，重命名是针对单个物品收费。如果手中持有 64 个物品，执行命令后将收取 64 x 45 = 2880 节操。

例如 ```/nu rename `&7&l好喝 的水` ```。

### 像素画粘贴
如果需要从单人世界复制像素画到喵窝（brainhole 维度），可联系*奈诺 `Aqua_nano`* 购买服务。

|类型|最小规模|收费|
|-|-|-|
| 平面像素画 | 6 幅1:1比例地图 | 20000 节操/每地图 |
| 立体像素画 | 2 幅1:1比例地图 | 50000 节操/每地图 |

+ **如何使用服务？**
  - 像素画可自行手工铺设，也可通过 [MapartCraft](https://bbs.craft.moe/d/1499-mapartcraft) 等第三方工具生成（可选立体化）。
  - 然后，利用 **Litematica 插件**，将像素画区域保存为 **投影文件**，发送给*奈诺* 。
    * 也可发送 Schematica、结构方块NBT文件（.nbt）或地图存档；但可能视情况加收一定服务费。
  - 粘贴之后，该绘画由你自由处置。展示或出售时，应标注原画作者。
+ **注意事项**
  - 限制级内容一律拒绝受理。
  - 严禁通过该服务刷取生存物资。
  - 地图一经粘贴，恕不更换（粘贴时出错者除外）。**购买服务前，请先确认像素画效果正常。**
  - 尽量避免扎堆粘贴。
+ 最新规则请见 [BBS帖子](https://bbs.nyaa.cat/d/1534)。


### 高级装备回收

通过在“无尽地狱”铸造/摇号获得的任意武器或辅助道具，如不满意，可联系*奈诺 `Aqua_nano`* 或管理员回收。

- <span style="color:#f44336;">红色稀有度（T5+）</span> —— 60000 节操

回收价格可能依「系统余额」动态调整。最新动态请见 [BBS帖子](https://bbs.nyaa.cat/d/1561-infinite-infernal)。

此服务受理时从「系统余额」直接拨款。

### 玩家提供的系统服务

玩家可以借助 Capcat、NyaaBank 等插件来提供系统级服务，并赚取节操。目前支持的服务：
- [开设银行](nyaa/economic/nyaabank)
- [购置、使用传送牌](space/plugins/capcat)

### 死亡惩罚

重生是需要代价的。**除`brainhole`维度外，在一切维度死亡均掉落。**  
重生本身不会扣除节操；但返回原地`/back`会。

### 其它收费项目

- `/suicide` 9998 节操 / 次  
与上述命令不同的是，扣除的 9998 节操**不会进入系统余额。**

## 在线奖励

**主条目：[PlayTimeTracker](space/plugins/playtimetracker.md)**

- **daily**——每日签到（固定值）
- **eco-up**——每日经济活跃（根据系统 balance 浮动）
- **daily2**——每日签到2（固定值）
- **week**——每周签到（根据系统 balance 浮动）
- **month**——每月签到（根据系统 balance 浮动）
- **activator**——每月活跃值贡献者奖励（固定值）

!> 如「系统余额」过低，相关奖励项将不能保证足额发放；陷入负值时，即停止支付，直至恢复到正值。

## 创造激励计划

主条目：[创造激励计划](nyaa/creation.md)

创造激励计划由管理员负责基本框架的建设和任务指引，并通过各种交流途径（Wiki、BBS、群组等）向玩家邀请，协调玩家完成具体任务。

如果参加[建造工程](nyaa/projects.md)，建设（手工）、材料与节操预算将由管理员根据建设进度逐步发放；工程量较小时，可能直接发放材料。  
建筑建设完成后，在门前留下建筑者的名牌以及购置费用（如有必要），以便日后管理员购置或其他玩家购置时支付相应的节操。

!> 请负责的玩家认真督促工程进度，谢绝拖延。

### 玩家自主的创造激励计划

玩家可以自主发起各类激励计划。激励计划需征得管理员认可；对于建造工程，还需取得土地所有者（如果有）的同意方可开工。
玩家自主激励计划可根据规模，向管理员申请一定的补贴。


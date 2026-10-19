# 科研词条对照表（内部 id ↔ 官方英文 ↔ 中文）

来源：DE Languages.bin 专用科研语言键，经 calamity-inc 自动提取；按完整语言键一一对应，禁止拆词或模糊匹配。

语言版本：44.1.2；提取提交：`f20f5879d01c9ac8bbbfa599710cd0b7a62ab101`。
源文件：[英文](https://raw.githubusercontent.com/calamity-inc/warframe-languages-bin-data/f20f5879d01c9ac8bbbfa599710cd0b7a62ab101/en.json)、[中文](https://raw.githubusercontent.com/calamity-inc/warframe-languages-bin-data/f20f5879d01c9ac8bbbfa599710cd0b7a62ab101/zh.json)。

覆盖：105 条官方词条记录，另列 3 条接口别名／自定义补充。包含全部个人限制、风险变量和两地任务变体，不限于本周轮换。

本表自动生成，供对照查询；图片中的自定义显示请修改同目录 `research-terms.md`。当前显示由线上共用科研解析器计算，保留已有自定义文案。
任务变体的 id 带 `CT_HEX:` 或 `CT_LAB:` 前缀，避免同名 key 在两地含义或数值不同而混淆；风险变量与任务变体分节列出。
没有同名官方语言键的接口别名另列，不借用无关词条充数。语言数据含游戏内部候选项，不表示所有条目都必定进入当前轮换。
重新生成：在 Runtime 目录执行 `node scripts/sync-research-terms-mapping.js`。更新官方源并生成：加 `--refresh`，需要代理时再加 `--proxy=http://127.0.0.1:10808`。

## 个人限制

共 32 条。

| 内部 id | 当前显示 | 官方英文 | 官方中文 | 官方描述 | 官方语言键 |
| --- | --- | --- | --- | --- | --- |
| AbilityLockout | 技能禁用 | Powerless | 技能禁用 | 小队击杀 50 名敌人前，所有技能均被禁止使用。 | /Lotus/Language/Conquest/PersonalMod_AbilityLockout |
| AnemicShields | 乏能护盾 | Anemic Shields | 乏能护盾 | 最大护盾和过载护盾不会超过 500。 | /Lotus/Language/Conquest/PersonalMod_AnemicShields |
| AntiGuard | 超宏降低 | Dropped Guard | 超宏衰减 | 战甲和友军超宏防护获取量减少 75% | /Lotus/Language/Conquest/PersonalMod_AntiGuard |
| AoeDebuff | 低收益 | Low Yield | 低收益 | 具有范围攻击的武器爆炸半径固定为 &#124;val&#124; 米。 | /Lotus/Language/Conquest/PersonalMod_AoeDebuff |
| Armorless | 无影响 | Fractured Armor | 破损护甲 | 施放技能会使护甲降低 10%，持续 10 秒。 | /Lotus/Language/Conquest/PersonalMod_Armorless |
| ChannelDrain | 导引耗能 | Channeled Greed | 贪婪导引 | 导引技能激活期间，最大护盾和过载护盾每秒都会降低。完全恢复需要 10 秒的冷却时间。 | /Lotus/Language/Conquest/PersonalMod_ChannelDrain |
| ComboCountChance | 钝重兵刃 | Dull Blades | 钝重兵刃 | 近战连击数几率减少 50% | /Lotus/Language/Conquest/PersonalMod_ComboCountChance |
| Conductive | 导电侵袭 | Conductive | 导电侵袭 | 每隔几秒就会受到 &lt;DT_ELECTRICITY&gt;电击伤害。 | /Lotus/Language/Conquest/PersonalMod_Conductive |
| ContactDamage | 二次伤害 | Secondary Wounds | 二次伤害 | 每次受到伤害时，获得 1 层 &lt;DT_PUNCTURE&gt;穿刺异常状态。 | /Lotus/Language/Conquest/PersonalMod_ContactDamage |
| DamageMomentum | 致命速率 | Terminal Velocity | 致命速率 | 静止不动时无法造成伤害。 | /Lotus/Language/Conquest/PersonalMod_DamageMomentum |
| DecayingFlesh | 永久损伤 | Permanent Injury | 永久损伤 | 受到生命值伤害时还会扣减最大生命上限 | /Lotus/Language/Conquest/PersonalMod_DecayingFlesh |
| EnergyStarved | 最大能量降低 | Constricted | 能量缩减 | 最大能量值减少 75% | /Lotus/Language/Conquest/PersonalMod_EnergyStarved |
| Exhaustion | 周围有敌人时不断掉蓝 | Energy Exhaustion | 能量枯竭 | 周围 10 米范围内的所有敌人使你每秒丢失 2 能量。 | /Lotus/Language/Conquest/PersonalMod_Exhaustion |
| ExposureCurse | 显露之诅 | Exposure Curse | 显露之诅 | 护盾被移除。 | /Lotus/Language/Conquest/PersonalMod_ExposureCurse |
| Framecurse | 放技能掉血（绕盾） | Framecurse Syndrome | 咒甲减益 | 激活一项技能时，会对你生命值造成 50 伤害，对护盾造成 150 伤害。 | /Lotus/Language/Conquest/PersonalMod_Framecurse |
| Gearless | 携带装备限制 | Gear Embargo | 携带装备限制 | 除曲翼枪械、原子摩托车和殁世机甲外，所有装备均受限制 | /Lotus/Language/Conquest/PersonalMod_Gearless |
| InfectedWounds | 感染伤口 | Infected Wounds | 感染伤口 | 每次受到伤害时，获得一层 &lt;DT_POISON_COLOR&gt;毒素异常状态。 | /Lotus/Language/Conquest/PersonalMod_InfectedWounds |
| Knifestep | 刀步症候群 | Knifestep Syndrome | 如履刀尖 | 移动时损失 2 点生命值。跳跃会暂停效果。 | /Lotus/Language/Conquest/PersonalMod_Knifestep |
| MaxAmmo | 补给短缺 | Undersupplied | 补给短缺 | 所有武器的弹药最大值减少 75% | /Lotus/Language/Conquest/PersonalMod_MaxAmmo |
| NoPets | 不让带同伴 | No Pets Allowed | 宠物禁入 | 禁用同伴 | /Lotus/Language/Conquest/PersonalMod_NoPets |
| OperatorLockout | 传识阻断 | Transference Distortion | 传识失真 | 无法传识到指挥官或漂泊者。 | /Lotus/Language/Conquest/PersonalMod_OperatorLockout |
| OverSensitive | 无影响 | Hypersensitive | 过敏受体 | 负面异常状态的持续时间增加到三倍 | /Lotus/Language/Conquest/PersonalMod_OverSensitive |
| RangeDebuff | 技能范围减半 | Shortened Reach | 咫尺之限 | 技能范围减少 &#124;val&#124;%。 | /Lotus/Language/Conquest/PersonalMod_RangeDebuff |
| Sanguine | 血色减益 | Sanguine Syndrome | 血色减益 | 每当你受到伤害时，还会陷入 &lt;DT_SLASH&gt;切割异常状态。 | /Lotus/Language/Conquest/PersonalMod_Sanguine |
| ScarcityCurse | 弹药枯竭 | Ammo Scarcity | 弹药枯竭 | 弹药逐渐耗尽。电池武器充能缓慢。 | /Lotus/Language/Conquest/PersonalMod_ScarcityCurse |
| ShieldDelay | 护盾恢复延迟提高 | Lethargic Shields | 嗜睡护盾 | 护盾充能延迟增加 &#124;val&#124;%。 | /Lotus/Language/Conquest/PersonalMod_ShieldDelay |
| Starvation | 弹药短缺 | Ammo Deficit | 弹药亏空 | 通过掉落和道具恢复的弹药减少 75%。 | /Lotus/Language/Conquest/PersonalMod_Starvation |
| TimeDilation | 缩短技能 | Abbreviated Abilities | 缩短技能 | 技能持续时间减少 &#124;val&#124;%。 | /Lotus/Language/Conquest/PersonalMod_TimeDilation |
| Vampyri | 吸血减益 | Vampyric Syndrome | 吸血减益 | 每秒流失生命值。击杀敌人可恢复生命值。 | /Lotus/Language/Conquest/PersonalMod_Vampyri |
| VitalEnergy | 震荡耗能 | Concussive Drain | 震荡耗能 | 每当生命值受到伤害，也会消耗最大能量的 5%。 | /Lotus/Language/Conquest/PersonalMod_VitalEnergy |
| VoidEnergyOverload | 技能过载 | Ability Overload | 技能超载 | 使用技能将在附近打开一道虚空裂隙 | /Lotus/Language/Conquest/PersonalMod_VoidEnergyOverload |
| Withering | 无影响 | Untreatable | 无法治愈 | 拾取无法提供治疗，并且无法拾取生命球。 | /Lotus/Language/Conquest/PersonalMod_Withering |

## 风险变量

共 36 条。

| 内部 id | 当前显示 | 官方英文 | 官方中文 | 官方描述 | 官方语言键 |
| --- | --- | --- | --- | --- | --- |
| AcceleratedEnemies | 敌人伤害更低但更肉 | Bold Venture | 激进冒险 | 敌人造成的伤害 -15%，受到的伤害 +15% ，但移动速度、攻击速度和射速 +15%。 | /Lotus/Language/Conquest/Condition_AcceleratedEnemies |
| AntiMaterialWeapons | 敌人伤害更高 | Commanding Culverins | 指挥型重型炮兵 | 暴戾重型炮兵装备的武器对超宏防护和殁世机甲造成 5 倍的伤害。 | /Lotus/Language/Conquest/Condition_AntiMaterialWeapons |
| ArcadeAutomata | 无影响 | Arcade Automata | 自动街机 | 敌人的枪械发射巨大且缓慢移动的球体，而不是他们平常的弹药。 | /Lotus/Language/Conquest/Condition_ArcadeAutomata |
| ArtilleryBeacons | 无影响 | Artillery Beacons | 炮击信标 | 炽蛇军敌人被击杀时会掉落炮击信标召唤轰炸。 | /Lotus/Language/Conquest/Condition_ArtilleryBeacons |
| BalloonFest | 气球敌人增多 | Balloonfest | 气球嘉年华 | 炽蛇军前哨气球数量更多，攻击和移动速度更快。 | /Lotus/Language/Conquest/Condition_BalloonFest |
| CompetitionSpillover | 随机Debuff | Competitive Streak | 竞争优势 | 在整个任务过程中，阿米尔和碧的"对战"模式将产生随机负面惩罚。 | /Lotus/Language/Conquest/Condition_CompetitionSpillover |
| Deflectors | 可出现守护卓越者 | Fortified Foes | 坚不可摧 | 可能会出现守护者卓越者敌人，包括守护者卓越者殁世机甲。 | /Lotus/Language/Conquest/Condition_Deflectors |
| DrainingResiduals | 无影响 | Devil's Bargain | 恶魔契约 | 敌人被击杀时 4 米范围内的友军会牺牲 50% 的弹药效率以换取 +25% 的射速。 | /Lotus/Language/Conquest/Condition_DrainingResiduals |
| EfervonFog | 毒雾 | Dense Fog | 浓雾 | 艾弗旺气体覆盖整个关卡。敌人可能会掉落提供短暂缓解的过滤器。 | /Lotus/Language/Conquest/Condition_EfervonFog |
| EmpoweredEnemies | 等比增防 | Proportional Resistance | 等比增防 | 敌人的生命值和护盾增加 100%，每拥有一个小队成员额外增加 50%，最多 300%。卓越者单位的部署更加频繁。 | /Lotus/Language/Conquest/Condition_EmpoweredEnemies |
| EnemyElementalEnhancement | 元素效力 | Elemental Potency | 元素效力 | 敌人造成 +100% 元素伤害，并对元素伤害有 +85% 抗性。 | /Lotus/Language/Conquest/Condition_EnemyElementalEnhancement |
| ExplosiveCrawlers | 无影响 | Explosive Potential | 易爆潜能 | 爆裂断肢取代蹒跚断肢。 | /Lotus/Language/Conquest/Condition_ExplosiveCrawlers |
| ExplosiveSummer | 过量炸药 | Excessive Explosives | 过量炸药 | 所有补给箱都被炸药桶替换。 | /Lotus/Language/Conquest/Condition_ExplosiveSummer |
| FactionSwarm_Scaldra | 无影响 | Scaldra Speed Run | 炽蛇军竞速 | 所有敌人被炽蛇军取代，并且移动的更快。 | /Lotus/Language/Conquest/Condition_FactionSwarm_Scaldra |
| FactionSwarm_Techrot | 无影响 | Techrot Speed Run | 科腐者竞速 | 所有敌人被科腐者取代，并且移动的更快。 | /Lotus/Language/Conquest/Condition_FactionSwarm_Techrot |
| FallFog | 浓雾之秋 | Foggy Fall | 浓雾之秋 | 迷雾限制了整个任务区的视野。 | /Lotus/Language/Conquest/Condition_FallFog |
| HeavyWarfare | 非重武减伤 | Heavy Warfare | 重装作战 | 敌人受到重型武器和热熔火箭炮的伤害增加 1.25 倍，其他来源的伤害降低 95%。敌人会掉落重型弹药包，重型武器的召回时间缩短至 5 秒。 | /Lotus/Language/Conquest/Condition_HeavyWarfare |
| HostileOvergrowth | 站着不动时受伤踉跄 | It's Alive | 它是活的 | 在地下，如果玩家停止移动，敌方增生物就会发起攻击。 | /Lotus/Language/Conquest/Condition_HostileOvergrowth |
| InfectedTechrot | 无影响 | Corrupted Flesh | 腐朽之躯 | 科腐者敌人被注入艾弗旺并随时间推移受到伤害。他们被击杀后会爆炸并留下致命的艾弗旺。 | /Lotus/Language/Conquest/Condition_InfectedTechrot |
| JadeSpring | 翠玉之灵 | Jade Spirits | 翠玉之灵 | 翠玉之灵徘徊在该区域。如果玩家靠近，它们就会追逐玩家并转变为翠玉光束。 | /Lotus/Language/Conquest/Condition_JadeSpring |
| MagneticHounds | 迷人弧犬 | Alluring Arcocanids | 迷人弧犬 | 当暴戾弧犬发起攻击时，它们会将战甲拉向自己。 | /Lotus/Language/Conquest/Condition_MagneticHounds |
| MeleeOnlyEnemies | 短兵相接 | Close Quarters | 短兵相接 | 只出现近战攻击的敌人。 | /Lotus/Language/Conquest/Condition_MeleeOnlyEnemies |
| MiasmiteHive | 无影响 | Miasmite Swarm | 自爆虫群 | 在任务过程中，科腐者自爆虫会从阴影中蜂拥而出。 | /Lotus/Language/Conquest/Condition_MiasmiteHive |
| MurmurIncursion | 加入低语者 | Beyond The Wall | 墙壁之外 | 低语者敌人加入炽蛇军和科腐者阵营。 | /Lotus/Language/Conquest/Condition_MurmurIncursion |
| PointBlank | 远离玩家的敌人无敌 | Myopic Munitions | 短视弹药 | 玩家距离敌人 15 米以内时，敌人才会受到伤害。 | /Lotus/Language/Conquest/Condition_PointBlank |
| Quicksand | 敌人死后减速周围玩家 | Entanglement | 牵连 | 被击杀敌人 4 米范围内的友军， 移动速度和跑酷速度会降低。 | /Lotus/Language/Conquest/Condition_Quicksand |
| RangedOnlyEnemies | 远程交战 | Ranged Engagements | 远程交战 | 只出现远程攻击的敌人。 | /Lotus/Language/Conquest/Condition_RangedOnlyEnemies |
| RegeneratingEnemies | 敌人自动回血 | Hostile Regeneration | 敌军复生 | 敌人的生命值会缓慢恢复。 | /Lotus/Language/Conquest/Condition_RegeneratingEnemies |
| RestrictedConsumables | 延迟供应 | Delayed Supply | 延迟供应 | 消耗品有 30 秒冷却时间。魅影，待命舰员以及曲翼枪械除外。 | /Lotus/Language/Conquest/Condition_RestrictedConsumables |
| RestrictedRespawns | 终局 | Finality | 终局 | 禁用自我复活。濒死的玩家只能通过击杀嘲讽低语来复活。死亡的玩家无法继续进行连续任务。 | /Lotus/Language/Conquest/Condition_RestrictedRespawns |
| SentientAdaptation | 适应异变 | Adaptive Aberrations | 适应异变 | 敌人受到元素伤害时产生相应的抗性。如果在 5 秒内没有受到该元素伤害，则抗性会消失。 | /Lotus/Language/Conquest/Condition_SentientAdaptation |
| ShieldedFoes | 敌人全体超宏 | Bolstered Belligerents | 强化好战 | 所有敌人获得相当于他们最大生命值 50% 的超宏防护。 | /Lotus/Language/Conquest/Condition_ShieldedFoes |
| Vanquisher | 卓越支援 | Eximus Reinforcements | 卓越支援 | 部署额外的卓越者敌人。 | /Lotus/Language/Conquest/Condition_Vanquisher |
| VoidAberration | 吸血吸蓝的无敌怪 | Vampyric Liminus | 吸血界影 | 行动缓慢且不死的双衍王境界影，能从过于接近的友军身上吸取生命和能量。 | /Lotus/Language/Conquest/Condition_VoidAberration |
| Voidburst | 无影响 | Postmortal Surges | 死后冲击 | 被击杀的敌人会爆发出虚空能量。 | /Lotus/Language/Conquest/Condition_Voidburst |
| WinterFrost | 厚冰 | Thick Ice | 厚冰 | 极寒卓越者护罩的耐久度是正常值的 30 倍。 | /Lotus/Language/Conquest/Condition_WinterFrost |

## 时光科研任务变体（CT_HEX）

共 15 条。

| 内部 id | 当前显示 | 官方英文 | 官方中文 | 官方描述 | 官方语言键 |
| --- | --- | --- | --- | --- | --- |
| CT_HEX:ChemicalNoise | 噪音抑制 | Noise Suppression | 噪音抑制 | 无人机在弗莱尔上方飞行，向他喷射艾弗旺气体。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_ChemicalNoise |
| CT_HEX:ContaminationZone | 屏住呼吸 | Hold Your Breath | 屏住呼吸 | 整个区域会随着玩家停留时间的延长而造成 &lt;DT_POISON_COLOR&gt;毒素伤害，地狱净化器附近区域除外。有些敌人可能会掉落过滤器，可用于创造额外稳定的临时安全区。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_ContaminationZone |
| CT_HEX:DisruptiveSounds | 驱散罩子 | Vamp Rock | 吸血摇滚 | 弗莱尔会创造一个力场，干扰玩家的技能，同时消耗能量以增强弗莱尔的生命值。当没有玩家在范围内时，弗莱尔会缓慢失去生命值。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_DisruptiveSounds |
| CT_HEX:DoubleTroubleLegacyte | 有丝分裂 | Mitosis | 有丝分裂 | 每轮产生两个传承种，需要两倍的捕获次数才能成功。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_DoubleTroubleLegacyte |
| CT_HEX:EscalateImmediately | 破坏补给 | Cache Crash | 破坏补给 | 任务开始时，触发打开补给箱的负面效果，一旦打开就会加剧。未能打开补给箱会导致完成任务所需的击杀数翻倍。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_EscalateImmediately |
| CT_HEX:ExplosiveEnergy | 无影响 | Miasmite Mash | 自爆虫浆 | 敌人死亡时掉落的自爆虫会立即冲向弗莱尔。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_ExplosiveEnergy |
| CT_HEX:FortifiedFoes | 封闭装甲 | Sealed Armor | 密闭装甲 | 非弱点命中对敌人造成的伤害降低 90%。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_FortifiedFoes |
| CT_HEX:GestatingTumors | 孢子增殖 | Sporogenesis | 孢子增殖 | 地狱净化器附近会出现科腐者肿瘤，每个活跃的肿瘤都会增加维生系统衰减的速度。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_GestatingTumors |
| CT_HEX:HighScalingLegacyte | 生长激素 | Growth Hormones | 生长激素 | 每一代传承种都更加强大，但同时也需要更长的时间来逃脱。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_HighScalingLegacyte |
| CT_HEX:HostileSecurity | 破坏之音 | Disruptive Sounds | 破坏之音 | 弗莱尔在自身周围发出一个干扰力场，干扰技能并消耗能量。如果范围内没有玩家，弗莱尔将流失生命值。他会根据范围内的玩家数量获得生命值。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_HostileSecurity |
| CT_HEX:MutatedEnemies | 平行进化 | Parallel Evolution | 平行进化 | 随着传承种进化，其他在场敌人也将获得新技能。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_MutatedEnemies |
| CT_HEX:TankReinforcements | 空降敌人 | Reinforcements | 支援 | 战斗过程中会有敌方援军抵达，首先是炽蛇军，然后是科腐者。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_TankReinforcements |
| CT_HEX:TankStrongArmor | 火箭筒才能打坦克 | Thermian Plating | 热熔装甲板 | 只有热熔火箭弹才能对坦克造成伤害。携带热熔火箭炮的增援部队将在战斗中持续出现。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_TankStrongArmor |
| CT_HEX:TankSuperToxic | 剧毒坦克 | Toxic Tank | 剧毒坦克 | 坦克拥有 &lt;DT_POISON_COLOR&gt;毒素光环，留下 &lt;DT_POISON_COLOR&gt;毒素尾迹，并且所有的攻击会造成 &lt;DT_POISON_COLOR&gt;毒素伤害。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_TankSuperToxic |
| CT_HEX:TechrotConjunction | 科腐围攻 | Pile-On | 科腐围攻 | 科腐者敌人会尝试近战攻击地狱净化器，接触后将其引爆，并使净化器污染增加 33%。 | /Lotus/Language/Conquest/MissionVariant_HexConquest_TechrotConjunction |

## 深层科研任务变体（CT_LAB）

共 22 条。

| 内部 id | 当前显示 | 官方英文 | 官方中文 | 官方描述 | 官方语言键 |
| --- | --- | --- | --- | --- | --- |
| CT_LAB:AlchemicalShields | 炼金难侵 | Alchemical Invulnerability | 炼金难侵 | 有 10% 敌人装备了不可穿透的元素屏障，只有对应元素的元素瓶才能摧毁屏障。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_AlchemicalShields |
| CT_LAB:DoubleTrouble | 每个导管多一个爆破，但总体更脆 | Double Demolishers | 双重爆破 | 两台爆破型殁世机甲会攻击任意导管，但它们的生命值降低。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_DoubleTrouble |
| CT_LAB:DuoAssassination | 双重接肢 | The Fragmented Two | 双重接肢 | 在最终战斗中对战两个接肢怪。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_DuoAssassination |
| CT_LAB:EnemyLink | 伤害链接 | Damage Link | 伤害链接 | 相距 10 米内的敌人形成一个伤害链接群体。任何对单个成员造成的伤害都会平均分摊到整个群体。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_EnemyLink |
| CT_LAB:EnvironmentalSystem | 危险区域 | Hazardous Areas | 危险区域 | 激活维生装置塔以为你的小队清除危险区域。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_EnvironmentalSystem |
| CT_LAB:EximusGrenadiers | 卓越者元素瓶 | Eximus Amphors | 卓越者元素瓶 | 卓越者敌人必定掉落元素瓶，但只有他们会掉落元素瓶。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_EximusGrenadiers |
| CT_LAB:FortifiedFoes | 封闭装甲 | Sealed Armor | 密闭装甲 | 非弱点命中对敌人造成的伤害降低 90%。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_FortifiedFoes |
| CT_LAB:FragileNodes | 导管可被敌人打炸 | Unified Purpose | 统一目标 | 敌人可以瞄准并摧毁导管。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_FragileNodes |
| CT_LAB:GrowingIncursion | 裂缝激增 | Fissure Cascade | 裂缝激增 | 裂缝在任务中形成，使得敌人的等级每 10 秒提升 1 级。消灭它们以防止等级增加。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_GrowingIncursion |
| CT_LAB:HarshWords | 无影响 | Barbed Glyphs | 带刺钥符 | 每个浮印在被收集时都会造成少量伤害。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_HarshWords |
| CT_LAB:HostileSecurity | 目标持续掉血 | Eroding Senses | 侵蚀感官 | 魔耳和魔瞳随着时间逐渐受损，收集所需的荧音浮印可暂停损伤并对它们进行部分修复。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_HostileSecurity |
| CT_LAB:HungryPillars | 辐化御敌 | Radioactive Breakdown | 辐化御敌 | 所有敌人都是无敌的，只有在受到辐射异常状态影响时才会受到伤害。辐射柱体随机出现并造成 &lt;DT_RADIATION&gt;辐射异常状态。  | /Lotus/Language/Conquest/MissionVariant_LabConquest_HungryPillars |
| CT_LAB:InfiniteTide | 无情肢潮 | Relentless Tide | 无情肢潮 | 断肢潮不会停止攻击。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_InfiniteTide |
| CT_LAB:LostInTranslation | 浮印膨胀 | Glyph Inflation | 浮印膨胀 | 安全系统需要两倍的荧音浮印才能激活。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_LostInTranslation |
| CT_LAB:MisguidedInstructions | 浮印陷阱 | Glyph Trap | 浮印陷阱 | 某些荧音浮印附有传送门陷阱，接触它时会被传送到 250 米以外的地方。传送门显性后持续 45 秒。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_MisguidedInstructions |
| CT_LAB:NecramechActivation | 敌人机甲增多 | Necramech Influx | 殁世机甲激增 | 殁世机甲出现的频率更高。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_NecramechActivation |
| CT_LAB:NecramechLockout | 敌意支援 | Hostile Support | 敌意支援 | 禁用维生装置塔运送系统。每 90 秒生成殁世机甲，击杀时掉落 6 个维生模块。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_NecramechLockout |
| CT_LAB:Reinforcements | 无影响 | Coordinated Front | 协调阵线 | 卓越者敌人出现并支援断肢潮和最终的接肢怪。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_Reinforcements |
| CT_LAB:SameTeam | 天使同行 | Angelic Cohort | 天使同行 | 虚空天使与最终的接肢怪并肩作战。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_SameTeam |
| CT_LAB:StickyFingers | 膨胀格鲁兹 | Engorged Gruzzlings | 暴食贪囤 | 所有贪囤断肢都是卓越者。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_StickyFingers |
| CT_LAB:UnpoweredCapsules | 寄生装置塔 | Parasitic Towers | 寄生装置塔 | 维生装置塔只有在其 15 米范围内杀死 20 名敌人后才会激活。  | /Lotus/Language/Conquest/MissionVariant_LabConquest_UnpoweredCapsules |
| CT_LAB:VolatileGrenades | 高危物资 | Hazardous Goods | 高危物资 | 携带元素瓶时会受到与之对应的元素伤害。 | /Lotus/Language/Conquest/MissionVariant_LabConquest_VolatileGrenades |

## 接口别名与自定义补充

共 3 条。

| 内部 id | 当前显示 | 官方英文 | 官方中文 | 官方描述 | 官方语言键 |
| --- | --- | --- | --- | --- | --- |
| DullBlades | 近战连击数获取减半 | Dull Blades | 钝重兵刃 | 近战连击数几率减少 50% | /Lotus/Language/Conquest/PersonalMod_ComboCountChance |
| EMPBlackHole | 无影响 | 无同名官方语言键 | 弧蛛牵引 | 未提供 | 接口 key／自定义显示；不做模糊匹配 |
| Undersupplied | 备弹降低 | 无同名官方语言键 | 弹药匮乏 | 未提供 | 接口 key／自定义显示；不做模糊匹配 |

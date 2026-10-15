# 紫卡市场词条显示名

标题必须使用 WFM slug（`riven-attributes-lkg.json` 里的 `slug` 字段）；`显示` 是紫卡市场卡片上的中文短文案。

可选字段：
- `近战显示`：同一 slug 在近战/zaw 武器上使用的文案（如射速/攻击速度、基础伤害/近战伤害）
- `参考英文名`：WFM 英文原名，便于对照
- `参考gameRef`：游戏内部 tag，便于对照

修改后发送 `wf重载 紫卡市场` 即可生效，无需重启 Bot。

## ammo_maximum
显示：备弹
别称：最大弹药值
参考英文名：Ammo Maximum
参考gameRef：WeaponAmmoMaxMod

## base_damage_/_melee_damage
显示：基伤
近战显示：基伤
参考英文名：Damage
参考gameRef：WeaponDamageAmountMod

## chance_to_gain_combo_count
显示：获取连击
参考英文名：Chance to Gain Combo Count
参考gameRef：WeaponMeleeComboPointsOnHitMod

## chance_to_gain_extra_combo_count
显示：额外连击
参考英文名：Additional Combo Count Chance
参考gameRef：WeaponMeleeComboBonusOnHitMod

## channeling_damage
显示：初始
参考英文名：Initial combo
参考gameRef：WeaponMeleeComboInitialBonusMod

## channeling_efficiency
显示：重效
参考英文名：Heavy Attack Efficiency
参考gameRef：WeaponMeleeComboEfficiencyMod

## cold_damage
显示：冰
参考英文名：Cold
参考gameRef：WeaponFreezeDamageMod

## combo_duration
显示：连击时间
参考英文名：Combo Duration
参考gameRef：ComboDurationMod

## critical_chance
显示：暴率
参考英文名：Critical Chance
参考gameRef：WeaponCritChanceMod

## critical_chance_on_slide_attack
显示：滑暴
参考英文名：Critical Chance for Slide Attack
参考gameRef：SlideAttackCritChanceMod

## critical_damage
显示：暴伤
参考英文名：Critical Damage
参考gameRef：WeaponCritDamageMod

## damage_vs_corpus
显示：对C
参考英文名：Damage to Corpus
参考gameRef：WeaponFactionDamageCorpus

## damage_vs_grineer
显示：对G
参考英文名：Damage to Grineer
参考gameRef：WeaponFactionDamageGrineer

## damage_vs_infested
显示：对I
参考英文名：Damage to Infested
参考gameRef：WeaponFactionDamageInfested

## electric_damage
显示：电
参考英文名：Electricity
参考gameRef：WeaponElectricityDamageMod

## finisher_damage
显示：处决
参考英文名：Finisher Damage
参考gameRef：WeaponMeleeFinisherDamageMod

## fire_rate_/_attack_speed
显示：射速
近战显示：攻速
参考英文名：Fire Rate / Attack Speed
参考gameRef：WeaponFireRateMod

## heat_damage
显示：火
参考英文名：Heat
参考gameRef：WeaponFireDamageMod

## impact_damage
显示：冲
参考英文名：Impact
参考gameRef：WeaponImpactDamageMod

## magazine_capacity
显示：弹匣
参考英文名：Magazine Capacity
参考gameRef：WeaponClipMaxMod

## multishot
显示：多重
参考英文名：Multishot
参考gameRef：WeaponFireIterationsMod

## projectile_speed
显示：投射
参考英文名：Projectile speed
参考gameRef：WeaponProjectileSpeedMod

## punch_through
显示：穿透
参考英文名：Punch Through
参考gameRef：WeaponPunctureDepthMod

## puncture_damage
显示：穿
参考英文名：Puncture
参考gameRef：WeaponArmorPiercingDamageMod

## range
显示：范围
参考英文名：Range
参考gameRef：WeaponMeleeRangeIncMod

## recoil
显示：后坐
参考英文名：Weapon Recoil
参考gameRef：WeaponRecoilReductionMod

## reload_speed
显示：装填
参考英文名：Reload Speed
参考gameRef：WeaponReloadSpeedMod

## slash_damage
显示：切
参考英文名：Slash
参考gameRef：WeaponSlashDamageMod

## status_chance
显示：触率
参考英文名：Status Chance
参考gameRef：WeaponStunChanceMod

## status_duration
显示：触时
参考英文名：Status Duration
参考gameRef：WeaponProcTimeMod

## toxin_damage
显示：毒
参考英文名：Toxin
参考gameRef：WeaponToxinDamageMod

## zoom
显示：变焦
参考英文名：Zoom
参考gameRef：WeaponZoomFovMod

<!-- 以下为融合词条（Riven Splicer / spliced attributes），来源 wiki.warframe.com/w/Riven_Mods。
     基础值/倾向计算在 packages/riven/src/analysis/spliced-attributes.js；这里只管查询别称与卡片显示。
     注意：`爆` 故意不给 Blast（它已经是暴击几率的既有别称），Blast 用 `爆炸`。 -->

## ammo_efficiency
显示：效率
别称：效率、弹药效率、弹效、子弹效率、ammo efficiency
别称：效率、弹药效率、弹效、子弹效率、ammo efficiency
参考英文名：Ammo Efficiency
参考gameRef：WeaponAmmoEfficiencyMod

## blast
显示：爆炸
别称：爆炸、爆炸伤害、炸裂、blast damage
别称：爆炸、爆炸伤害、炸裂、blast damage
参考英文名：Blast Damage
参考gameRef：WeaponBlastDamageMod

## corrosive
显示：腐蚀
别称：腐蚀、腐蚀伤害、腐朽、扒皮、腐、corrosive damage
别称：腐蚀、腐蚀伤害、腐朽、扒皮、腐、corrosive damage
参考英文名：Corrosive Damage
参考gameRef：WeaponCorrosiveDamageMod

## damage_to_orokin
显示：对O
别称：对O、对奥罗金、对奥罗金伤害、对奥罗金的伤害、对orokin、对O佬、对O老、orokin damage
别称：对O、对奥罗金、对奥罗金伤害、对奥罗金的伤害、对orokin、对O佬、对O老、orokin damage
参考英文名：Damage vs. Orokin
参考gameRef：WeaponFactionDamageOrokin

## damage_to_scaldra
显示：对炽蛇
别称：对炽蛇、对炽蛇军伤害、对炽蛇军的伤害、对炽蛇军、对赤蛇军伤害、对赤蛇军的伤害、对赤蛇军、对赤蛇、炽蛇、赤蛇、scaldra damage
别称：对炽蛇、对炽蛇军伤害、对炽蛇军的伤害、对炽蛇军、对赤蛇军伤害、对赤蛇军的伤害、对赤蛇军、对赤蛇、炽蛇、赤蛇、scaldra damage
参考英文名：Damage vs. Scaldra
参考gameRef：WeaponFactionDamageScaldra

## damage_to_techrot
显示：对科腐
别称：对科腐、对科腐者伤害、对科腐者的伤害、对科腐者、科腐、对科、科、techrot damage
别称：对科腐、对科腐者伤害、对科腐者的伤害、对科腐者、科腐、对科、科、techrot damage
参考英文名：Damage vs. Techrot
参考gameRef：WeaponFactionDamageTechrot

## gas
显示：毒气
别称：毒气、毒气伤害、gas damage
别称：毒气、毒气伤害、gas damage
参考英文名：Gas Damage
参考gameRef：WeaponGasDamageMod

## heavy_attack_wind_up_speed
显示：重击速度
别称：重击速度、重击准备速度、重型攻击准备速度、蓄力速度、重击前摇、蓄力前摇、重型攻击蓄力速度、重型攻击速度、heavy attack wind up speed
别称：重击速度、重击准备速度、重型攻击准备速度、蓄力速度、重击前摇、蓄力前摇、重型攻击蓄力速度、重型攻击速度、heavy attack wind up speed
参考英文名：Heavy Attack Wind Up Speed
参考gameRef：WeaponMeleeHeavyAttackWindUpMod

## magnetic
显示：磁力
别称：磁力、磁力伤害、磁、magnetic damage
别称：磁力、磁力伤害、磁、magnetic damage
参考英文名：Magnetic Damage
参考gameRef：WeaponMagneticDamageMod

## melee_damage_on_heavy_attack
显示：重击基伤
别称：重击基伤、重击伤害、重型攻击伤害、重型震地伤害、重型攻击基伤、melee damage on heavy attack
别称：重击基伤、重击伤害、重型攻击伤害、重型震地伤害、重型攻击基伤、melee damage on heavy attack
参考英文名：Melee Damage On Heavy Attack
参考gameRef：WeaponMeleeHeavyAttackDamageMod

## parry_angle
显示：格挡
别称：格挡、格挡角度、抵挡角度、弹反角度、parry angle
别称：格挡、格挡角度、抵挡角度、弹反角度、parry angle
参考英文名：Parry Angle
参考gameRef：WeaponMeleeParryAngleMod

## radiation
显示：辐射
别称：辐射、辐射伤害、放射、放射性、辐、radiation damage
别称：辐射、辐射伤害、放射、放射性、辐、radiation damage
参考英文名：Radiation Damage
参考gameRef：WeaponRadiationDamageMod

## magazine_reloaded_s_when_holstered
显示：收起自动换弹
别称：收起自动换弹、收起时装填、收起时换弹、自动装填、自动换弹、reload while holstered
别称：收起自动换弹、收起时装填、收起时换弹、自动装填、自动换弹、reload while holstered
参考英文名：Reload While Holstered
参考gameRef：WeaponReloadWhileHolsteredMod

## slam_attack_damage
显示：震地伤害
别称：震地攻击伤害、地震攻击伤害、震地伤害、震地攻击、震地、震击、slam attack damage、slam damage
别称：震地攻击伤害、地震攻击伤害、震地伤害、震地攻击、震地、震击、slam attack damage、slam damage
参考英文名：Slam Attack Damage
参考gameRef：WeaponMeleeSlamAttackDamageMod

## status_damage
显示：异况伤害
别称：异况伤害、异常状态伤害、异况、状态伤害、dot伤害、status damage
别称：异况伤害、异常状态伤害、异况、状态伤害、dot伤害、status damage
参考英文名：Status Damage
参考gameRef：WeaponStatusDamageMod

## viral
显示：病毒
别称：病毒、病毒伤害、易伤、疾病、viral damage
别称：病毒、病毒伤害、易伤、疾病、viral damage
参考英文名：Viral Damage
参考gameRef：WeaponViralDamageMod

## weak_point_critical_chance
显示：弱点暴率
别称：弱点暴率、弱点暴击几率、弱点暴击率、弱点爆率、爆头暴击几率、爆头暴击率、爆头爆率、爆头暴率、弱爆、爆暴、爆爆、weakpoint critical chance
别称：弱点暴率、弱点暴击几率、弱点暴击率、弱点爆率、爆头暴击几率、爆头暴击率、爆头爆率、爆头暴率、弱爆、爆暴、爆爆、weakpoint critical chance
参考英文名：Weakpoint Critical Chance
参考gameRef：WeaponWeakpointCritChanceMod

## weak_point_damage
显示：弱点
别称：弱点、弱点伤害、爆头伤害、爆头倍率、爆头、weakpoint damage
别称：弱点、弱点伤害、爆头伤害、爆头倍率、爆头、weakpoint damage
参考英文名：Weakpoint Damage
参考gameRef：WeaponWeakpointDamageMod

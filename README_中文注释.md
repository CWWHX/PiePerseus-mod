# 配置文件中文注释

> 文中数据修改（原始配置表中为“-1”）在“-1”下为不进行修改的状态，修改数据改成0或者正整数，例如修改敌人数据可以改成0，修改我方武器数据伤害可以改成20000。
>
> 原始配置表中为false的，是功能修改开关，只可以修改为false、true，表示关和开。
>
> 表中的移除buff功能建议先不要用，会导致关卡结算卡加载。

```bash
"Aircraft"修改敌我双方小飞机: {
  "Enabled"功能开关
  "Accuracy"命中率，原始值范围0-50
  "AccuracyGrowth"命中率成长值，原始典型值0
  "AttackPower"攻击力，原始值范围0-50
  "AttackPowerGrowth"攻击力成长值，原始值范围0-3000
  "CrashDamage"碰撞伤害，原始值范围1-2000
  "Hp"最大生命值，原始值范围13-99999
  "HpGrowth"生命值成长值，原始值范围0-200000
  "Speed"速度，原始值范围20-120
},

"Enemies"修改敌人数据: {
  "Enabled"功能开关
  "AntiAir"防空，原始值范围0-200000
  "AntiAirGrowth"防空成长值，原始值范围0-10000
  "AntiSubmarine"反潜，原始值范围0-999
  "Armor"装甲，原始值范围0-42
  "ArmorGrowth"装甲成长值，原始典型值0
  "Cannon"炮击，原始值范围0-2333333
  "CannonGrowth"炮击成长值，原始值范围0-10000
  "Evasion"机动，原始值范围0-999
  "EvasionGrowth"机动成长值，原始值范围0-10000
  "Hit"命中，原始值范围0-9999
  "HitGrowth"命中成长值，原始值范围0-10000
  "Hp"耐久，原始值范围0-99999999
  "HpGrowth"耐久成长值，原始值范围0-910000
  "Luck"幸运，原始值范围0-100
  "LuckGrowth"幸运成长值，原始值范围0-10000
  "Reload"装填，原始值范围0-9999
  "ReloadGrowth"装填成长值，原始典型值0
  "RemoveBuffs"移除buff
  "RemoveEquipment"移除装备
  "RemoveSkill"移除技能
  "Speed"航速，原始值范围0-300
  "SpeedGrowth"航速，原始典型值0
  "Torpedo"雷击，原始值范围0-2333333
  "TorpedoGrowth"雷击成长值，原始值范围0-15655
},

"Weapons"修改我方武器: {
  "Enabled"功能开关
  "Damage"武器伤害，原始值范围0-30000
  "ReloadMax"最大装填时间，原始值范围0-999999
},
  
"Spoof"伪装，自欺欺人: {
  "Enabled"功能开关
  "Name"指挥官名字
  "Id"UID
  "Lv"等级
},

"Misc"杂项: {
  "Enabled"功能开关
  "ExerciseGodmode"演习无敌
  "FastStageMovement"快速移动
  "Skins"全皮肤
  "AutoRepeatLimit"连续作战次数
  "ChatCommands"聊天框命令
  "RemoveBBAnimation"移除舰炮开火动画
  "RemoveMoraleWarning"移除舰娘低心情警告
  "RemoveHardModeStatLimit"移除困难关卡限制
  "RemoveNSFWArts"移除瑟瑟
}
```

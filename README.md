# MUDGameGit
人物类character

属性：
Id
名字name
等级level
体力值health_point
魔力值 mana_point
防御力physical_defence
法术抗性 magic_defence
攻击力	attack_point
暴击值 critic
暴击伤害 critical_damage
命中值 hit_value
闪避值 dodge_value
速度 speed
暴击抗性 critical_defence
效果抗性 cc_defence

行为：
攻击 attack
技能 skill
逃跑 escape
交谈 communicate
死亡 die

主角类 hero
属性：
物品 item
装备栏 equipment_slot

行为：
使用道具 use_item
休息 rest
拾取 pick
移动 move

npc类（人物类）npc
属性：
刷新条件 recur_condition
掉落物 drop_item
仇恨值 hostility

行为：
掉落物品 dropout

物品类 item
属性：
价值 value
Id
数量 number

行为：
使用 be_used


装备类（物品）equipment
属性：
防御力补正additional_physical_defence
法术抗性补正 additional_magic_defence
攻击力补正	additional_attack_point
暴击值补正 additional_critic
暴击伤害补正 additional_critical_damage
命中值补正 additional_hit_value
闪避值补正 additional_dodge_value
速度补正 additional_speed
暴击抗性补正 additional_critical_defence
效果抗性补正 additional_cc_defence

行为：
被穿戴 equip
被卸下 unequip

房间类 room
属性：
上面的房间 up_room
下面的房间 down_room
左边的房间 left_room
右边的房间right_room
隐藏的房间 hidden_room
内部的物品 contained_item
内部的人物 contained_character

行为：
人物更新 update_character
物品更新 update_item
野怪刷新 renew_enemy

指令类：
属性：
世界时间 global_time

行为：
读取指令 load_command
执行指令 execute_command

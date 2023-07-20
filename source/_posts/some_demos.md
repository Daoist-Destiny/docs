---
title: some demo
---


```go
func initArmsMap() {
	ArmsMap = map[int]model.ArmsStruct{
		0: model.ArmsStruct{
			ArmsId:      0,
			ArmsName:    "空",
			ArmsInfo:    "",
			ArmsStatus:  model.StatusStruct{0, 0, 0, 0, 0, 0},
			ArmsSkillId: 0,
			ArmsBuy:     0,
			ArmsSale:    0,
			ArmsLevel:   0,
		},
		800: model.ArmsStruct{
			ArmsId:   800,
			ArmsName: "夺志剑",
			ArmsInfo: "无视御劲，吸取精力",
			ArmsStatus: model.StatusStruct{
				UserJin:     15,
				UserMu:      15,
				UserShui:    15,
				UserHuo:     15,
				UserTu:      15,
				UserYinYang: 0,
			},
			ArmsSkillId: 800,
			ArmsBuy:     0,
			ArmsSale:    0,
			ArmsLevel:   0,
		},
	}
```


```go
EnemysMap = map[int]model.EnemysStruct{
		111: {EnemyId: 111, EnemyName: "金钱会外围", EnemyStatus: model.StatusStruct{85, 10, 10, 10, 10, 1}, EnemySkillIdList: []int{1101}, EnemyEx: 50, EnemyGoodsId: []int{1111, 1311, 1511}},
		112: {112, "金钱会喽喽", model.StatusStruct{190, 15, 15, 15, 15, 1}, []int{1101, 1102}, 100, []int{1111, 1311, 1511, 1121, 1321, 1521}},
		113: {113, "金钱会打手", model.StatusStruct{295, 20, 20, 20, 20, 1}, []int{2101, 1102}, 150, []int{1121, 1321, 1521, 1131, 1331, 1531}},
		114: {114, "金钱会头目", model.StatusStruct{400, 25, 25, 25, 25, 1}, []int{2101, 1102}, 200, []int{1131, 1331, 1531, 1141, 1341, 1541}},
		115: {115, "金钱会堂主", model.StatusStruct{505, 30, 30, 30, 30, 1}, []int{3101, 1102}, 250, []int{1141, 1341, 1541, 1151, 1351, 1551}},
		116: {116, "金钱会香主", model.StatusStruct{610, 35, 35, 35, 35, 1}, []int{3101, 1102}, 250, []int{1151, 1351, 1551, 1161, 1361, 1561}},
		117: {117, "金钱会三当家", model.StatusStruct{715, 40, 40, 40, 40, 1}, []int{4101, 1102}, 300, []int{1161, 1361, 1561, 1170}},
		118: {118, "金钱会二当家", model.StatusStruct{820, 45, 45, 45, 45, 1}, []int{4101, 1102}, 350, []int{1161, 1361, 1561, 1170, 1180}},
		119: {119, "金钱会大当家", model.StatusStruct{925, 50, 50, 50, 50, 1}, []int{4101, 1102}, 400, []int{1161, 1361, 1561, 1170, 1180, 1190}},

		121: {121, "青狼教外围", model.StatusStruct{10, 85, 10, 10, 10, 1}, []int{1201}, 50, []int{1211, 1311, 1411}},
		122: {122, "青狼教喽喽", model.StatusStruct{15, 190, 15, 15, 15, 1}, []int{1201, 1202}, 100, []int{1211, 1311, 1411, 1221, 1321, 1421}},
		123: {123, "青狼教打手", model.StatusStruct{20, 295, 20, 20, 20, 1}, []int{2201, 1202}, 150, []int{1221, 1321, 1421, 1231, 1331, 1431}},
		124: {124, "青狼教头目", model.StatusStruct{25, 400, 25, 25, 25, 1}, []int{2201, 1202}, 200, []int{1231, 1331, 1431, 1241, 1341, 1441}},
		125: {125, "青狼教堂主", model.StatusStruct{30, 505, 30, 30, 30, 1}, []int{3201, 1202}, 250, []int{1241, 1341, 1441, 1251, 1351, 1451}},
		126: {126, "青狼教香主", model.StatusStruct{35, 610, 35, 35, 35, 1}, []int{3201, 1202}, 250, []int{1251, 1351, 1451, 1261, 1361, 1461}},
		127: {127, "青狼教三当家", model.StatusStruct{40, 715, 40, 40, 40, 1}, []int{4201, 1202}, 300, []int{1261, 1361, 1461, 1270}},
		128: {128, "青狼教二当家", model.StatusStruct{45, 820, 45, 45, 45, 1}, []int{4201, 1202}, 350, []int{1261, 1361, 1461, 1270, 1280}},
		129: {129, "青狼教大当家", model.StatusStruct{50, 925, 50, 50, 50, 1}, []int{4201, 1202}, 400, []int{1261, 1361, 1461, 1270, 1280, 1290}},

		131: {131, "黑虎派外围", model.StatusStruct{10, 10, 85, 10, 10, 1}, []int{1301}, 50, []int{1311, 1111, 1211}},
		132: {132, "黑虎派喽喽", model.StatusStruct{15, 15, 190, 15, 15, 1}, []int{1301, 1302}, 100, []int{1311, 1111, 1211, 1321, 1121, 1221}},
		133: {133, "黑虎派打手", model.StatusStruct{20, 20, 295, 20, 20, 1}, []int{2301, 1302}, 150, []int{1321, 1121, 1221, 1331, 1131, 1231}},
		134: {134, "黑虎派头目", model.StatusStruct{25, 25, 400, 25, 25, 1}, []int{2301, 1302}, 200, []int{1331, 1131, 1231, 1341, 1141, 1241}},
		135: {135, "黑虎派堂主", model.StatusStruct{30, 30, 505, 30, 30, 1}, []int{3301, 1302}, 250, []int{1341, 1141, 1241, 1351, 1151, 1251}},
		136: {136, "黑虎派香主", model.StatusStruct{35, 35, 610, 35, 35, 1}, []int{3301, 1302}, 250, []int{1351, 1151, 1251, 1361, 1161, 1261}},
		137: {137, "黑虎派三当家", model.StatusStruct{40, 40, 715, 40, 40, 1}, []int{4301, 1302}, 300, []int{1361, 1161, 1261, 1370}},
		138: {138, "黑虎派二当家", model.StatusStruct{45, 45, 820, 45, 45, 1}, []int{4301, 1302}, 350, []int{1361, 1161, 1261, 1370, 1380}},
		139: {139, "黑虎派大当家", model.StatusStruct{50, 50, 925, 50, 50, 1}, []int{4301, 1302}, 400, []int{1361, 1161, 1261, 1370, 1380, 1390}},

		141: {141, "火头帮外围", model.StatusStruct{10, 10, 10, 85, 10, 1}, []int{1401}, 50, []int{1411, 1211, 1511}},
		142: {142, "火头帮喽喽", model.StatusStruct{15, 15, 15, 190, 15, 1}, []int{1401, 1402}, 100, []int{1411, 1211, 1511, 1421, 1221, 1521}},
		143: {143, "火头帮打手", model.StatusStruct{20, 20, 20, 295, 20, 1}, []int{2401, 1402}, 150, []int{1421, 1221, 1521, 1431, 1231, 1531}},
		144: {144, "火头帮头目", model.StatusStruct{25, 25, 25, 400, 25, 1}, []int{2401, 1402}, 200, []int{1431, 1231, 1531, 1441, 1241, 1541}},
		145: {145, "火头帮堂主", model.StatusStruct{30, 30, 30, 505, 30, 1}, []int{3401, 1402}, 250, []int{1441, 1241, 1541, 1451, 1251, 1551}},
		146: {146, "火头帮香主", model.StatusStruct{35, 35, 35, 610, 35, 1}, []int{3401, 1402}, 250, []int{1451, 1251, 1551, 1461, 1261, 1561}},
		147: {147, "火头帮三当家", model.StatusStruct{40, 40, 40, 715, 40, 1}, []int{4401, 1402}, 300, []int{1461, 1261, 1561, 1470}},
		148: {148, "火头帮二当家", model.StatusStruct{45, 45, 45, 820, 45, 1}, []int{4401, 1402}, 350, []int{1461, 1261, 1561, 1470, 1480}},
		149: {149, "火头帮大当家", model.StatusStruct{50, 50, 50, 925, 50, 1}, []int{4401, 1402}, 400, []int{1461, 1261, 1561, 1470, 1480, 1490}},

		151: {151, "地鼠门外围", model.StatusStruct{10, 10, 10, 10, 85, 1}, []int{1501}, 50, []int{1511, 1111, 1141}},
		152: {152, "地鼠门喽喽", model.StatusStruct{15, 15, 15, 15, 190, 1}, []int{1501, 1502}, 100, []int{1511, 1111, 1141, 1521, 1121, 1241}},
		153: {153, "地鼠门打手", model.StatusStruct{20, 20, 20, 20, 295, 1}, []int{2501, 1502}, 150, []int{1521, 1121, 1241, 1531, 1131, 1341}},
		154: {154, "地鼠门头目", model.StatusStruct{25, 25, 25, 25, 400, 1}, []int{2501, 1502}, 200, []int{1531, 1131, 1341, 1541, 1141, 1341}},
		155: {155, "地鼠门堂主", model.StatusStruct{30, 30, 30, 30, 505, 1}, []int{3501, 1502}, 250, []int{1541, 1141, 1341, 1551, 1151, 1351}},
		156: {156, "地鼠门香主", model.StatusStruct{35, 35, 35, 35, 610, 1}, []int{3501, 1502}, 250, []int{1551, 1151, 1351, 1561, 1161, 1361}},
		157: {157, "地鼠门三当家", model.StatusStruct{40, 40, 40, 40, 715, 1}, []int{4501, 1502}, 300, []int{1561, 1161, 1361, 1570}},
		158: {158, "地鼠门二当家", model.StatusStruct{45, 45, 45, 45, 820, 1}, []int{4501, 1502}, 350, []int{1561, 1161, 1361, 1570, 1580}},
		159: {159, "地鼠门大当家", model.StatusStruct{50, 50, 50, 50, 925, 1}, []int{4501, 1502}, 400, []int{1561, 1161, 1361, 1570, 1580, 1590}},
	}
```

```go
package data

import "demo-x/model"

var GameData model.GameDataStruct
var FeaturesMap map[int]model.FeaturesStruct
var LevelNameMap map[int]string

func InitGameData() {
	GameData = model.GameDataStruct{
		UserName:  "",
		UserLevel: 0,
		UserEx:    0,
		UserStatus: model.StatusStruct{
			UserJin:     0,
			UserMu:      0,
			UserShui:    0,
			UserHuo:     0,
			UserTu:      0,
			UserYinYang: 0,
		},
		UserBag: model.BagsStruct{
			UseId: 0,
			Bag:   [64]model.CaseStruct{},
		},
		UserArmBag: model.ArmsBagStruct{
			UseId: 0,
			Bag:   [64]model.ArmsCaseStruct{},
		},
		UserSaveId:        0,
		UserMapsIdList:    []int{1, 2},
		UserPageIdMap:     map[int]int{},
		UserOwnBodySkill:  [100]model.SkillsStruct{},
		UserOwnHeartSkill: [100]model.SkillsStruct{},
		//		UserQuestDoing:    map[int]model.QuestsInfoStruct{},
		//		UserQuestsDone:    map[int]model.QuestsInfoStruct{},
		UserMateriel: model.MaterielsStruct{
			HeartSkillId: 0,
			BodySkillId:  0,
			ArmFirstId:   0,
			ArmSecondId:  0,
			ArmThirdId:   0,
		},
	}
}
func initLevelNameMap() {
	LevelNameMap = map[int]string{
		1:   "唤金使者",
		2:   "呼水使者",
		3:   "遣木使者",
		4:   "派火使者",
		5:   "敕土使者",
		11:  "皓灵道士",
		12:  "五灵道士",
		13:  "青灵道士",
		14:  "丹灵道士",
		15:  "玄灵道士",
		21:  "太白星君",
		22:  "岁星星君",
		23:  "辰星星君",
		24:  "荧惑星君",
		25:  "镇星星君",
		310: "上章真君",
		311: "重光真君",
		//313: "蓐收真君",
		320: "阏逢真君",
		321: "旃蒙真君",
		//323: "句芒真君",
		331: "玄黓真君",
		330: "昭阳真君",
		//333: "玄冥真君",
		341: "柔兆真君",
		340: "强圉真君",
		//343: "祝庸真君",
		351: "著雍真君",
		350: "屠维真君",
		//353: "后土真君",
		42: "东方青帝青灵始老九炁天君",
		44: "南方赤帝丹灵真老三炁天君",
		45: "中央黄帝玄灵黄老一炁天君",
		41: "西方白帝皓灵皇老七炁天君",
		43: "北方黑帝五灵玄老五炁天君",
	}
}

func initStatusMap() {
	FeaturesMap = map[int]model.FeaturesStruct{
		1: model.FeaturesStruct{
			FeaturesId:          1,
			FeaturesName:        "神兵煌煌",
			FeaturesInfo:        "神兵煌煌",
			FeaturesAsk:         "拥有一件法宝才是重中之重",
			FeaturesGiveGoodsId: 800,
		},

		2: model.FeaturesStruct{
			FeaturesId:          2,
			FeaturesName:        "高朋满座",
			FeaturesInfo:        "高朋满座",
			FeaturesAsk:         "如果能有一群志同道合的朋友也是也是幸事(当前版本不建议选择)",
			FeaturesGiveGoodsId: 802,
		},
		3: model.FeaturesStruct{
			FeaturesId:          3,
			FeaturesName:        "道法自然",
			FeaturesInfo:        "道法自然",
			FeaturesAsk:         "一门高深的道法乃是安身立命之本",
			FeaturesGiveGoodsId: 801,
		},
		4: model.FeaturesStruct{
			FeaturesId:          4,
			FeaturesName:        "愚钝非凡",
			FeaturesInfo:        "愚钝非凡",
			FeaturesAsk:         "愚钝非凡",
			FeaturesGiveGoodsId: 0,
		},
		5: model.FeaturesStruct{
			FeaturesId:          5,
			FeaturesName:        "天元一气",
			FeaturesInfo:        "天元一气",
			FeaturesAsk:         "天元一气",
			FeaturesGiveGoodsId: 0,
		},
		6: model.FeaturesStruct{
			FeaturesId:          6,
			FeaturesName:        "三元汇聚",
			FeaturesInfo:        "三元汇聚",
			FeaturesAsk:         "三元汇聚",
			FeaturesGiveGoodsId: 0,
		},
		7: model.FeaturesStruct{
			FeaturesId:          7,
			FeaturesName:        "五行调和",
			FeaturesInfo:        "五行调和",
			FeaturesAsk:         "五行调和",
			FeaturesGiveGoodsId: 0,
		},
	}

}
```

```go
GoodsMap = map[int]model.GoodsInfoStruct{
		0:   {0, "", "空", 0, 0, 0, "", goodsFunc0},
		1:   {1, "心法", "《纳元诀》", 0, 0, 0, "入门心法", goodsFunc1},
		801: {801, "功法", "《混元一气功》", 0, 0, 0, "将低于平均值的属性，提升至平均值", goodsFunc801},
		802: {802, "道具", "唤符", 0, 0, 0, "召唤随机人选帮助攻击", goodsFunc802},
		803: {803, "丹药", "仙灵丹", 0, 0, 0, "增加经验", goodsFunc0},

		1111: {1111, "丹药", "金灵丹（残品）", 0, 0, 0, "残品金系丹药，炼化后增加5点金属性", func(active bool) (bool, string) { goodsAddJin(5); return true, "增加30点金属性" }},
		1121: {1121, "丹药", "金灵丹（次品）", 0, 0, 0, "次品金系丹药，炼化后增加30点金属性", func(active bool) (bool, string) { goodsAddJin(30); return true, "增加30点金属性" }},
		1131: {1131, "丹药", "金灵丹（凡品）", 0, 0, 0, "凡品金系丹药，炼化后增加55点金属性", func(active bool) (bool, string) { goodsAddJin(55); return true, "增加55点金属性" }},
		1141: {1141, "丹药", "金灵丹（中品）", 0, 0, 0, "中品金系丹药，炼化后增加80点金属性", func(active bool) (bool, string) { goodsAddJin(80); return true, "增加80点金属性" }},
		1151: {1151, "丹药", "金灵丹（精品）", 0, 0, 0, "精品金系丹药，炼化后增加105点金属性", func(active bool) (bool, string) { goodsAddJin(105); return true, "增加105点金属性" }},
		1161: {1161, "丹药", "金灵丹（仙品）", 0, 0, 0, "仙品金系丹药，炼化后增加130点金属性", func(active bool) (bool, string) { goodsAddJin(130); return true, "增加130点金属性" }},

		1170: {1170, "心法", "金系心法", 0, 0, 0, "金系心法", goodsFunc0},
		1180: {1180, "功法", "金系功法", 0, 0, 0, "金系功法", goodsFunc0},
		1190: {1190, "道具", "金系武器", 0, 0, 0, "获得金系武器", goodsFunc0},

		1211: {1211, "丹药", "木灵丹（残品）", 0, 0, 0, "残品木系丹药，炼化后增加5点木属性", func(active bool) (bool, string) { goodsAddMu(5); return true, "增加30点木属性" }},
		1221: {1221, "丹药", "木灵丹（次品）", 0, 0, 0, "次品木系丹药，炼化后增加30点木属性", func(active bool) (bool, string) { goodsAddMu(30); return true, "增加30点木属性" }},
		1231: {1231, "丹药", "木灵丹（凡品）", 0, 0, 0, "凡品木系丹药，炼化后增加55点木属性", func(active bool) (bool, string) { goodsAddMu(55); return true, "增加55点木属性" }},
		1241: {1241, "丹药", "木灵丹（中品）", 0, 0, 0, "中品木系丹药，炼化后增加80点木属性", func(active bool) (bool, string) { goodsAddMu(80); return true, "增加80点木属性" }},
		1251: {1251, "丹药", "木灵丹（精品）", 0, 0, 0, "精品木系丹药，炼化后增加105点木属性", func(active bool) (bool, string) { goodsAddMu(105); return true, "增加105点木属性" }},
		1261: {1261, "丹药", "木灵丹（仙品）", 0, 0, 0, "仙品木系丹药，炼化后增加130点木属性", func(active bool) (bool, string) { goodsAddMu(130); return true, "增加130点木属性" }},

		1270: {1270, "心法", "木系心法", 0, 0, 0, "木系心法", goodsFunc0},
		1280: {1280, "功法", "木系功法", 0, 0, 0, "木系功法", goodsFunc0},
		1290: {1290, "道具", "木系武器", 0, 0, 0, "获得木系武器", goodsFunc0},

		1311: {1311, "丹药", "水灵丹（残品）", 0, 0, 0, "残品水系丹药，炼化后增加5点水属性", func(active bool) (bool, string) { goodsAddShui(5); return true, "增加30点水属性" }},
		1321: {1321, "丹药", "水灵丹（次品）", 0, 0, 0, "次品水系丹药，炼化后增加30点水属性", func(active bool) (bool, string) { goodsAddShui(30); return true, "增加30点水属性" }},
		1331: {1331, "丹药", "水灵丹（凡品）", 0, 0, 0, "凡品水系丹药，炼化后增加55点水属性", func(active bool) (bool, string) { goodsAddShui(55); return true, "增加55点水属性" }},
		1341: {1341, "丹药", "水灵丹（中品）", 0, 0, 0, "中品水系丹药，炼化后增加80点水属性", func(active bool) (bool, string) { goodsAddShui(80); return true, "增加80点水属性" }},
		1351: {1351, "丹药", "水灵丹（精品）", 0, 0, 0, "精品水系丹药，炼化后增加105点水属性", func(active bool) (bool, string) { goodsAddShui(105); return true, "增加105点水属性" }},
		1361: {1361, "丹药", "水灵丹（仙品）", 0, 0, 0, "仙品水系丹药，炼化后增加130点水属性", func(active bool) (bool, string) { goodsAddShui(130); return true, "增加130点水属性" }},

		1370: {1370, "心法", "水系心法", 0, 0, 0, "水系心法", goodsFunc0},
		1380: {1380, "功法", "水系功法", 0, 0, 0, "水系功法", goodsFunc0},
		1390: {1390, "道具", "水系武器", 0, 0, 0, "获得水系武器", goodsFunc0},

		1411: {1411, "丹药", "火灵丹（残品）", 0, 0, 0, "残品火系丹药，炼化后增加5点火属性", func(active bool) (bool, string) { goodsAddHuo(5); return true, "增加30点火属性" }},
		1421: {1421, "丹药", "火灵丹（次品）", 0, 0, 0, "次品火系丹药，炼化后增加30点火属性", func(active bool) (bool, string) { goodsAddHuo(30); return true, "增加30点火属性" }},
		1431: {1431, "丹药", "火灵丹（凡品）", 0, 0, 0, "凡品火系丹药，炼化后增加55点火属性", func(active bool) (bool, string) { goodsAddHuo(55); return true, "增加55点火属性" }},
		1441: {1441, "丹药", "火灵丹（中品）", 0, 0, 0, "中品火系丹药，炼化后增加80点火属性", func(active bool) (bool, string) { goodsAddHuo(80); return true, "增加80点火属性" }},
		1451: {1451, "丹药", "火灵丹（精品）", 0, 0, 0, "精品火系丹药，炼化后增加105点火属性", func(active bool) (bool, string) { goodsAddHuo(105); return true, "增加105点火属性" }},
		1461: {1461, "丹药", "火灵丹（仙品）", 0, 0, 0, "仙品火系丹药，炼化后增加130点火属性", func(active bool) (bool, string) { goodsAddHuo(130); return true, "增加130点火属性" }},

		1470: {1470, "心法", "火系心法", 0, 0, 0, "火系心法", goodsFunc0},
		1480: {1480, "功法", "火系功法", 0, 0, 0, "火系功法", goodsFunc0},
		1490: {1490, "道具", "火系武器", 0, 0, 0, "获得火系武器", goodsFunc0},

		1511: {1511, "丹药", "土灵丹（残品）", 0, 0, 0, "残品土系丹药，炼化后增加5点土属性", func(active bool) (bool, string) { goodsAddTu(5); return true, "增加30点土属性" }},
		1521: {1521, "丹药", "土灵丹（次品）", 0, 0, 0, "次品土系丹药，炼化后增加30点土属性", func(active bool) (bool, string) { goodsAddTu(30); return true, "增加30点土属性" }},
		1531: {1531, "丹药", "土灵丹（凡品）", 0, 0, 0, "凡品土系丹药，炼化后增加55点土属性", func(active bool) (bool, string) { goodsAddTu(55); return true, "增加55点土属性" }},
		1541: {1541, "丹药", "土灵丹（中品）", 0, 0, 0, "中品土系丹药，炼化后增加80点土属性", func(active bool) (bool, string) { goodsAddTu(80); return true, "增加80点土属性" }},
		1551: {1551, "丹药", "土灵丹（精品）", 0, 0, 0, "精品土系丹药，炼化后增加105点土属性", func(active bool) (bool, string) { goodsAddTu(105); return true, "增加105点土属性" }},
		1561: {1561, "丹药", "土灵丹（仙品）", 0, 0, 0, "仙品土系丹药，炼化后增加130点土属性", func(active bool) (bool, string) { goodsAddTu(130); return true, "增加130点土属性" }},

		1570: {1570, "心法", "土系心法", 0, 0, 0, "土系心法", goodsFunc0},
		1580: {1580, "功法", "土系功法", 0, 0, 0, "土系功法", goodsFunc0},
		1590: {1590, "道具", "土系武器", 0, 0, 0, "获得土系武器", goodsFunc0},
```

```go
MapsMap = map[int]model.MapsStruct{
		0:  {MapId: 0, MapName1: "", MapName2: "", MapName3: "", MapLevelMin: 0, MapLevelMax: 0, MapInfo: "", MapEnemyIdList: nil},
		1:  {1, "中州", "三才宗", "书房", 0, 0, "三才宗书房", nil},
		2:  {2, "中州", "三才宗", "后山", 3, 5, "三才宗后山", []int{111, 121, 131, 141, 151}},
		11: {11, "中州", "金钱会", "外围", 5, 20, "金钱会外围领地", []int{111, 112, 113}},
		12: {12, "中州", "金钱会", "据点", 15, 30, "金钱会据点", []int{114, 115, 116}},
		13: {13, "中州", "金钱会", "总舵", 25, 40, "金钱会总舵，万分小心", []int{117, 118, 119}},
		21: {21, "中州", "青狼教", "外围", 5, 20, "青狼教外围领地", []int{121, 122, 123}},
		22: {22, "中州", "青狼教", "据点", 15, 30, "青狼教据点", []int{124, 125, 126}},
		23: {23, "中州", "青狼教", "总舵", 25, 40, "青狼教总舵，万分小心", []int{127, 128, 129}},
		31: {31, "中州", "黑虎派", "外围", 5, 20, "黑虎派外围领地", []int{131, 132, 133}},
		32: {32, "中州", "黑虎派", "据点", 15, 30, "黑虎派据点", []int{134, 135, 136}},
		33: {33, "中州", "黑虎派", "总舵", 25, 40, "黑虎派总舵，万分小心", []int{137, 138, 139}},
		41: {41, "中州", "火头帮", "外围", 5, 20, "火头帮外围领地", []int{141, 142, 143}},
		42: {42, "中州", "火头帮", "据点", 15, 30, "火头帮据点", []int{144, 145, 146}},
		43: {43, "中州", "火头帮", "总舵", 25, 40, "火头帮总舵，万分小心", []int{147, 148, 149}},
		51: {51, "中州", "地鼠门", "外围", 5, 20, "地鼠门外围领地", []int{151, 152, 153}},
		52: {52, "中州", "地鼠门", "据点", 15, 30, "地鼠门据点", []int{154, 155, 156}},
		53: {53, "中州", "地鼠门", "总舵", 25, 40, "地鼠门总舵，万分小心", []int{157, 158, 159}},
	}
```

```go

var SkillsMap map[int]model.SkillsStruct
var EnemySkillsMap map[int]model.SkillsStruct

func initSkills() {

	SkillsMap = map[int]model.SkillsStruct{
		0: {
			SkillsId:         0,
			SkillsName:       "未运转",
			SkillsInfo:       "尚未运转",
			SkillType:        "",
			SkillTypeId:      0,
			SkillsFunc:       enemyNull,
			SkillsUseActive:  0,
			SkillsUseByOther: 0,
		},

		1: {
			SkillsId:    1,
			SkillsName:  "纳元诀",
			SkillsInfo:  "三才宗入门心法，调用后可以缓慢增加修为。",
			SkillType:   "心法",
			SkillTypeId: 1,
			SkillsFunc: func(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
				//	if GameData.UserQuestDoing[1].QuestsCondition[1].QuestsCellCount == 0 {
				//		GameData.UserQuestDoing[1].QuestsCondition[1].QuestsCellCount = 1
				//	}
				if active {
					if !Skill1Active {

						Skill1Active = true
						go func() {
							for {
								GameData.UserEx++
								time.Sleep(1 * time.Second)
								if Skill1Active == false {
									break
								}
							}
						}()
						return true, AStatus, BStatus
					} else {
						//Skill1Active = true
						//已经运行，不能再运行，报错
						return false, AStatus, BStatus
					}
				} else {
					Skill1Active = false
					return true, AStatus, BStatus
				}
			},
			SkillsUseActive:  0,
			SkillsUseByOther: 1,
		},
		//1级别 法术01
		101: {101, "灵咒术", "运转灵韵，消耗100点气力，造成2倍破体的伤害", "功法", 2, Skill1x01, 1, 1},
		102: {102, "小还术", "运转灵韵，消耗一成气力，恢复2倍精力", "功法", 2, Skill1x02, 1, 1},
		401: {401, "灵杀术", "运转灵韵，消耗500点气力，造成20倍破体的伤害", "功法", 2, Skill4x01, 1, 1},
		800: {800, "萃取", "造成1倍破体（无视御劲）的伤害，并将伤害值作为精力护盾", "功法", 2, Skill800, 1, 1},
		801: {801, "混元一气功", "运转灵韵，放弃防御，造成一倍破体加御劲的伤害", "功法", 2, Skill801, 1, 1},
		999: {999, "普通攻击", "造成1倍破体的伤害", "功法", 2, Skill999, 1, 1},
	}

	EnemySkillsMap = map[int]model.SkillsStruct{
		// 1级  金系 法术01
		1101: {SkillsId: 1101, SkillsName: "金咒术", SkillsInfo: "运转金属性灵韵，消耗100点气力，造成2倍破体的伤害", SkillType: "功法", SkillTypeId: 2, SkillsFunc: Skill1x01, SkillsUseActive: 1, SkillsUseByOther: 1},
		1201: {1201, "木咒术", "运转木属性灵韵，消耗100点气力，造成2倍破体的伤害", "功法", 2, Skill1x01, 1, 1},
		1301: {1301, "水咒术", "运转水属性灵韵，消耗100点气力，造成2倍破体的伤害", "功法", 2, Skill1x01, 1, 1},
		1401: {1401, "火咒术", "运转火属性灵韵，消耗100点气力，造成2倍破体的伤害", "功法", 2, Skill1x01, 1, 1},
		1501: {1501, "土咒术", "运转土属性灵韵，消耗100点气力，造成2倍破体的伤害", "功法", 2, Skill1x01, 1, 1},
		// 1级  金系 法术02
		1102: {1102, "金复术", "运转金属性灵韵，消耗一成气力，恢复2倍精力", "功法", 2, Skill1x02, 1, 1},
		1202: {1202, "木复术", "运转木属性灵韵，消耗一成气力，恢复2倍精力", "功法", 2, Skill1x02, 1, 1},
		1302: {1302, "水复术", "运转水属性灵韵，消耗一成气力，恢复2倍精力", "功法", 2, Skill1x02, 1, 1},
		1402: {1402, "火复术", "运转火属性灵韵，消耗一成气力，恢复2倍精力", "功法", 2, Skill1x02, 1, 1},
		1502: {1502, "土复术", "运转土属性灵韵，消耗一成气力，恢复2倍精力", "功法", 2, Skill1x02, 1, 1},

		2101: {2101, "金击术", "运转金属性灵韵，消耗200点气力，造成5倍破体的伤害", "功法", 2, Skill2x01, 1, 1},
		2201: {2201, "木击术", "运转木属性灵韵，消耗200点气力，造成5倍破体的伤害", "功法", 2, Skill2x01, 1, 1},
		2301: {2301, "水击术", "运转水属性灵韵，消耗200点气力，造成5倍破体的伤害", "功法", 2, Skill2x01, 1, 1},
		2401: {2401, "火击术", "运转火属性灵韵，消耗200点气力，造成5倍破体的伤害", "功法", 2, Skill2x01, 1, 1},
		2501: {2501, "土击术", "运转土属性灵韵，消耗200点气力，造成5倍破体的伤害", "功法", 2, Skill2x01, 1, 1},

		3101: {3101, "金爆术", "运转金属性灵韵，消耗300点气力，造成10倍破体的伤害", "功法", 2, Skill3x01, 1, 1},
		3201: {3201, "木爆术", "运转木属性灵韵，消耗300点气力，造成10倍破体的伤害", "功法", 2, Skill3x01, 1, 1},
		3301: {3301, "水爆术", "运转水属性灵韵，消耗300点气力，造成10倍破体的伤害", "功法", 2, Skill3x01, 1, 1},
		3401: {3401, "火爆术", "运转火属性灵韵，消耗300点气力，造成10倍破体的伤害", "功法", 2, Skill3x01, 1, 1},
		3501: {3501, "土爆术", "运转土属性灵韵，消耗300点气力，造成10倍破体的伤害", "功法", 2, Skill3x01, 1, 1},

		4101: {4101, "金杀术", "运转金属性灵韵，消耗500点气力，造成20倍破体的伤害", "功法", 2, Skill4x01, 1, 1},
		4201: {4201, "木杀术", "运转木属性灵韵，消耗500点气力，造成20倍破体的伤害", "功法", 2, Skill4x01, 1, 1},
		4301: {4301, "水杀术", "运转水属性灵韵，消耗500点气力，造成20倍破体的伤害", "功法", 2, Skill4x01, 1, 1},
		4401: {4401, "火杀术", "运转火属性灵韵，消耗500点气力，造成20倍破体的伤害", "功法", 2, Skill4x01, 1, 1},
		4501: {4501, "土杀术", "运转土属性灵韵，消耗500点气力，造成20倍破体的伤害", "功法", 2, Skill4x01, 1, 1},
	}
}

func enemyNull(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {

	return active, AStatus, BStatus

}

func Skill999(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	if BStatus.Def <= AStatus.Atk {
		BStatus.Hp = BStatus.Hp - (AStatus.Atk - BStatus.Def)
	}
	return active, AStatus, BStatus
}
func Skill801(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	if BStatus.Def <= AStatus.Atk+AStatus.Def {
		BStatus.Hp = BStatus.Hp - (AStatus.Atk + AStatus.Def - BStatus.Def)
	}
	return active, AStatus, BStatus
}

func Skill800(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {

	BStatus.Hp = BStatus.Hp - AStatus.Atk
	AStatus.Hp = AStatus.Hp + AStatus.Atk
	return true, AStatus, BStatus

}

func Skill1x01(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	if AStatus.Mp >= 100 {
		if BStatus.Def <= AStatus.Atk*2 {
			BStatus.Hp = BStatus.Hp - (AStatus.Atk*2 - BStatus.Def)
			AStatus.Mp = AStatus.Mp - 100
		} else {
			AStatus.Mp = AStatus.Mp - 100
		}
		return active, AStatus, BStatus
	} else {
		return false, AStatus, BStatus
	}
}
func Skill2x01(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	if AStatus.Mp >= 200 {
		if BStatus.Def <= AStatus.Atk*5 {
			BStatus.Hp = BStatus.Hp - (AStatus.Atk*5 - BStatus.Def)
			AStatus.Mp = AStatus.Mp - 200
		} else {
			AStatus.Mp = AStatus.Mp - 200
		}
		return active, AStatus, BStatus
	} else {
		return false, AStatus, BStatus
	}
}
func Skill3x01(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	if AStatus.Mp >= 300 {
		if BStatus.Def <= AStatus.Atk*10 {
			BStatus.Hp = BStatus.Hp - (AStatus.Atk*10 - BStatus.Def)
			AStatus.Mp = AStatus.Mp - 300
		} else {
			AStatus.Mp = AStatus.Mp - 300
		}
		return active, AStatus, BStatus
	} else {
		return false, AStatus, BStatus
	}
}

func Skill4x01(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	if AStatus.Mp >= 500 {
		if BStatus.Def <= AStatus.Atk*20 {
			BStatus.Hp = BStatus.Hp - (AStatus.Atk*20 - BStatus.Def)
			AStatus.Mp = AStatus.Mp - 500
		} else {
			AStatus.Mp = AStatus.Mp - 500
		}
		return active, AStatus, BStatus
	} else {
		return false, AStatus, BStatus
	}
}

func Skill1x02(active bool, AStatus, BStatus model.PrintStatus) (bool, model.PrintStatus, model.PrintStatus) {
	//astatus自己，bstatus 对方
	mp := AStatus.Mp / 10
	AStatus.Hp = AStatus.Hp + 2*mp
	AStatus.Mp = AStatus.Mp - mp
	return active, AStatus, BStatus
}

var Skill1Active bool = false

func CheckSkillOwn(skillsInfo model.SkillsStruct) bool {
	status := false
	var skillsList [100]model.SkillsStruct

	if skillsInfo.SkillTypeId == 1 {
		skillsList = GameData.UserOwnHeartSkill
	} else {
		skillsList = GameData.UserOwnBodySkill
	}
	for _, s := range skillsList {

		if s.SkillsId == skillsInfo.SkillsId {
			status = true
			break
		}
	}
	return status
}
```


```go
func VeriftSave() bool {
	statusCode := true
	file, err := os.Open(conf.SaveFile)
	if err != nil {
		statusCode = false
	}
	defer file.Close()
	return statusCode
}

func InitData() {

}

func LoadData() {

	file, err := os.Open(conf.SaveFile)

	tools.CheckErr(err)
	defer file.Close()
	// 创建一个解码器
	decoder := gob.NewDecoder(file)
	// 解码数据并存储到新的切片
	err = decoder.Decode(&data.GameData)
	tools.CheckErr(err)

	//刷新技能，用于在更新任务后刷新已经学会的技能
	freshSkillsList()
	//自动运转功法
	activeSkills()

}
func freshSkillsList() {
	//刷新技能，用于在更新任务后刷新已经学会的技能

	for i := 0; i < data.GameData.MAXUserOwnHeartSkillId; i++ {
		//panic(gconv.String(data.GameData.UserOwnHeartSkill[i])+gconv.String(data.SkillsMap[data.GameData.UserOwnHeartSkill[i].SkillsId]))

		data.GameData.UserOwnHeartSkill[i] = data.SkillsMap[data.GameData.UserOwnHeartSkill[i].SkillsId]
	}
	for i := 0; i < data.GameData.MAXUserOwnBodySkillId; i++ {
		data.GameData.UserOwnBodySkill[i] = data.SkillsMap[data.GameData.UserOwnBodySkill[i].SkillsId]
	}
}
func QuitGame() {
	SaveData()
	os.Exit(0)
}
func activeSkills() {

	userUserMateriel := data.GameData.UserMateriel
	ActiveSkills(data.SkillsMap[userUserMateriel.HeartSkillId])
	ActiveSkills(data.SkillsMap[userUserMateriel.BodySkillId])
	ActiveSkills(data.SkillsMap[data.ArmsMap[userUserMateriel.ArmFirstId].ArmsSkillId])
	ActiveSkills(data.SkillsMap[data.ArmsMap[userUserMateriel.ArmSecondId].ArmsSkillId])
	ActiveSkills(data.SkillsMap[data.ArmsMap[userUserMateriel.ArmThirdId].ArmsSkillId])

}

func SaveData() {
	os.Mkdir(conf.SaveBakDir, 0755)
	file, err := os.Create(conf.SaveFile)

	tools.CheckErr(err)
	defer file.Close()
	encoder := gob.NewEncoder(file)
	err = encoder.Encode(data.GameData)
	tools.CheckErr(err)
}

func LevelUp() {
	for {
		if data.GameData.UserEx >= data.GameData.UserLevel*100 {
			data.GameData.UserEx = data.GameData.UserEx - data.GameData.UserLevel*100
			data.GameData.UserLevel = data.GameData.UserLevel + 1
			switch data.GameData.StatusAddModel {
			case 1:
				if data.GameData.UserLevel%5 == 0 {
					statusAdd([5]int{5, 5, 5, 5, 5})
				}
			case 2:
				statusAdd([5]int{5, 5, 5, 5, 5})
			case 11:
				statusAdd([5]int{17, 2, 2, 2, 2})

			case 12:
				statusAdd([5]int{2, 17, 2, 2, 2})
			case 13:
				statusAdd([5]int{2, 2, 17, 2, 2})
			case 14:
				statusAdd([5]int{2, 2, 2, 17, 2})
			case 15:
				statusAdd([5]int{2, 2, 2, 2, 17})
			case 21:
				statusAdd([5]int{7, 2, 7, 2, 7})
			case 22:
				statusAdd([5]int{2, 7, 7, 7, 2})
			case 23:
				statusAdd([5]int{7, 7, 7, 2, 2})
			case 24:
				statusAdd([5]int{2, 7, 2, 7, 7})
			case 25:
				statusAdd([5]int{7, 2, 2, 7, 7})
			}
		}
		time.Sleep(1 * time.Second)
	}
}
func statusAdd(arr [5]int) {
	data.GameData.UserStatus.UserJin = data.GameData.UserStatus.UserJin + arr[0]
	data.GameData.UserStatus.UserMu = data.GameData.UserStatus.UserMu + arr[1]
	data.GameData.UserStatus.UserShui = data.GameData.UserStatus.UserShui + arr[2]
	data.GameData.UserStatus.UserHuo = data.GameData.UserStatus.UserHuo + arr[3]
	data.GameData.UserStatus.UserTu = data.GameData.UserStatus.UserTu + arr[4]

}
func getUserStatus(id, y int) {
	nameList := []rune(data.GameData.UserName)
	c := 0
	for i := 0; i < len(nameList); i++ {
		c = c + gconv.Int(nameList[i])

	}

	if id == 5 {
		switch c % 5 {
		case 0:
			data.GameData.UserStatus = model.StatusStruct{17, 2, 2, 2, 2, y}
			data.GameData.StatusAddModel = 11
		case 1:
			data.GameData.UserStatus = model.StatusStruct{2, 17, 2, 2, 2, y}
			data.GameData.StatusAddModel = 12
		case 2:
			data.GameData.UserStatus = model.StatusStruct{2, 2, 17, 2, 2, y}
			data.GameData.StatusAddModel = 13
		case 3:
			data.GameData.UserStatus = model.StatusStruct{2, 2, 2, 17, 2, y}
			data.GameData.StatusAddModel = 14
		case 4:
			data.GameData.UserStatus = model.StatusStruct{2, 2, 2, 2, 17, y}
			data.GameData.StatusAddModel = 15
		}
	} else {
		switch c % 5 {
		case 0:

			data.GameData.UserStatus = model.StatusStruct{7, 2, 7, 2, 7, y}
			data.GameData.StatusAddModel = 21
		case 1:
			data.GameData.UserStatus = model.StatusStruct{2, 7, 7, 7, 2, y}
			data.GameData.StatusAddModel = 22
		case 2:
			data.GameData.UserStatus = model.StatusStruct{7, 7, 7, 2, 2, y}
			data.GameData.StatusAddModel = 23
		case 3:
			data.GameData.UserStatus = model.StatusStruct{2, 7, 2, 7, 7, y}
			data.GameData.StatusAddModel = 24
		case 4:
			data.GameData.UserStatus = model.StatusStruct{7, 2, 2, 7, 7, y}
			data.GameData.StatusAddModel = 25
		}
	}
}
func GetUserStatus(id int) {
	y := grand.N(0, 1)

	switch id {
	case 4:
		data.GameData.UserStatus = model.StatusStruct{1, 1, 1, 1, 1, y}
		data.GameData.StatusAddModel = 1
	case 5:

		getUserStatus(5, y)
	case 6:

		getUserStatus(6, y)
	case 7:
		data.GameData.UserStatus = model.StatusStruct{5, 5, 5, 5, 5, y}
		data.GameData.StatusAddModel = 2

	}

}

func GetAllPrintStatus(status model.StatusStruct) model.PrintStatus {
	//panic(status.UserJin + status.UserMu + status.UserShui + status.UserHuo + status.UserTu)
	//血量（HP）：
	//HP = (金属性值 * 1.5) + (木属性值 * 1.2) + (水属性值 * 0.8) + (火属性值 * 1.1) + (土属性值 * 1.3) + 基础血量值
	//其中，金属性值、木属性值、水属性值、火属性值和土属性值表示角色对应属性的数值。基础血量值表示角色本身的体质和基础生命值，例如100。
	//
	//法力值（MP）：
	//MP = (金属性值 * 0.8) + (木属性值 * 1.5) + (水属性值 * 1.5) + (火属性值 * 1.2) + (土属性值 * 1.1) + 基础法力值
	//其中，金属性值、木属性值、水属性值、火属性值和土属性值表示角色对应属性的数值。基础法力值表示角色本身的精神和基础法力值，例如50。
	//
	//攻击力（ATK）：
	//ATK = (金属性值 * 1.2) + (木属性值 * 1.5) + (水属性值 * 1.1) + (火属性值 * 1.3) + (土属性值 * 1.1) + 基础攻击力值
	//其中，金属性值、木属性值、水属性值、火属性值和土属性值表示角色对应属性的数值。基础攻击力值表示角色本身的力量和基础攻击力值，例如50。
	//
	//防御力（DEF）：
	//DEF = (金属性值 * 1.3) + (木属性值 * 1.1) + (水属性值 * 1.2) + (火属性值 * 1.1) + (土属性值 * 1.5) + 基础防御力值
	//其中，金属性值、木属性值、水属性值、火属性值和土属性值表示角色对应属性的数值。基础防御力值表示角色本身的体魄和基础防御力值，例如30。
	y := status.UserYinYang
	j := status.UserJin
	m := status.UserMu
	s := status.UserShui
	h := status.UserHuo
	t := status.UserTu
	hp := 15*j + 12*m + 8*s + 11*h + 13*t + 10000
	mp := 8*j + 15*m + 15*s + 12*h + 11*t + 5000
	atk := 12*j + 15*m + 11*s + 13*h + 11*t + 50
	def := 13*j + 11*m + 12*s + 11*h + 15*t + 30
	var printStatus model.PrintStatus
	if y == 1 {
		printStatus = model.PrintStatus{
			hp, mp, atk, def,
		}
	} else {
		printStatus = model.PrintStatus{
			mp, hp, def, atk,
		}
	}
	return printStatus
}

func GetPrintStatus() model.PrintStatus {

	status := data.GameData.UserStatus
	printStatus := GetAllPrintStatus(status)
	return printStatus

}
func GetLevelName() string {
	//获取职阶

	userLevel := data.GameData.UserLevel
	nameList := []rune(data.GameData.UserName)
	c := 0
	for i := 0; i < len(nameList); i++ {
		c = c + gconv.Int(nameList[i])

	}
	levelType := c % 5 //得到金木水火土

	levelCode := userLevel / 20 //{0,1,2,3,4,5}
	levelName := ""
	switch levelCode {
	case 3:
		levelName = data.LevelNameMap[levelCode*100+(levelType+1)*10+data.GameData.UserStatus.UserYinYang]

	default:
		levelName = data.LevelNameMap[levelCode*10+levelType+1]
	}

	//panic(data.LevelNameMap[levelCode*10+levelType+1])
	return levelName
}
```



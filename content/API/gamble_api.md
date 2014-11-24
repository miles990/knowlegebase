/*
Title: Gamble API
*/


	 說明	 Type	 參數1	 參數6	 	 		 			 	
 通用	 	 	 	 	 	 		 			 	
 Client To Server	 GM指令	 1004	 CurrID	 	 	 		 			 	
 Server To Client	 GM指令回傳	 1005	 1OK	 	 	 		 			 	
 Server To Client	 錯誤回傳	 1100	 ErrorID	 	 	 		 			 	
 	 	 	 	 	 	 	 	 	 		 	
 登入	 	 	 	 	 	 	 	 	 		 	
 Client To Server	 登入	 1101	 LoginCode	 RegistCode	 	 	 	 	 		 	
 Server To Client	 登入回傳	 1102	 CurrID	 UID	 CID	 1	 	 	 		 	
 Client To Server	 登出	 1103	 CurrID	 	 	 	 	 	 		 	
 Server To Client	 登出成功	 1104	 1	 	 	 	 	 	 		 	
 Server To Client	 重新登入	 1105	 	 	 	 	 	 	 		 	
 Client To Server	 設定暱稱	 1106	 CurrID	 NickName	 	 	 	 	 		 	
 Server To Client	 設定暱稱結果	 1107	 Number	 	 	 	 	 	 		 	
 Client To Server	 取得基本資料	 1108	 CurrID	 	 	 	 	 	 		 	
 Server To Client	 基本資料回傳	 1109	 Level	 Exp	 Money	 IsRegist	 HaveSaveCash	 	 		 	
 Client To Server	 取得玩家資訊	 1110	 CurrID	 FindUID	 FindCID	 	 	 	 		 	
 Server To Client	 取得玩家資訊回傳	 1111	 Json字串	 	 	 	 	 	 		 	
 Client To Server	 綁定註冊帳號	 1112	 CurrID	 RegistCode	 	 	 	 	 		 	
 Server To Client	 綁定註冊帳號回傳	 1113	 Status	 	 	 	 	 	 		 	
 Client To Server	 取得等級資訊	 1114	 CurrID	 	 	 	 	 	 		 	
 Server To Client	 取得等級資訊回傳	 1115	 Json字串	 	 	 	 	 	 		 	
 Client To Server	 取得個人資訊	 1116	 CurrID	 	 	 	 	 	 		 	
 Server To Client	 取得個人資訊回傳	 1117	 Json字串	 	 	 	 	 	 		 	
 機台頁面操作	 	 	 	 	 	 		 			 	
 Client To Server	 取得機台頁	 2001	 CurrID	 GameType	 Room	 		 			 	
 Server To Client	 取得機台頁回傳	 2002	 Count	 UID	 CID	 NickName	 GameType	 Room	 Index	 Status	 KeepStartTime	 …
 Client To Server	 進入機台確認	 2003	 CurrID	 GameType	 Room	 Index	 	 			 	
 Server To Client	 進入機台確認回傳	 2004	 Status	 	 	 		 			 	
 Client To Server	 進入機台	 2005	 CurrID	 GameType	 Room	 Index		 			 	
 Server To Client	 進入機台回傳	 2006	 Status	 GameType	 Room	 Index		 			 	
 Client To Server	 離開機台	 2007	 CurrID	 	 	 		 			 	
 Server To Client	 離開機台回傳	 2008	 1	 	 	 		 			 	
 Client To Server	 保留機台	 2009	 CurrID	 	 	 		 			 	
 Server To Client	 保留機台回傳	 2010	 Status	 	 	 		 			 	
 Client To Server	 隨機進入機台	 2011	 CurrID	 GameType	 Room	 		 			 	
 Server To Client	 隨機進入機台錯誤回傳	 2012	 Status	 	 	 		 			 	
 Client To Server	 取得自己的保留機台	 2013	 CurrID	 	 	 		 			 	
 Server To Client	 取得自己的保留機台回傳	 2014	 Status	 GameType	 Room	 Index		 		 	 	 	 	 
 	 	 	 	 	 	 		 		 	 	 	 	 
 海底世界	 	 	 	 	 	 		 		 	 	 	 	 
 Client To Server	 海底世界下注	 3001	 CurrID	 OneLineMoney	 GMFreeIconCount	 GMBonusIconCount	 GMHaveBigWin	 		 	 	 	 	 
 Server To Client	 海底世界下注回傳	 3002	 Status	 WinMoney	 NowMoney	 Icon x 15	 FreeStatus	 FreeTimes	 
BonusStatus
 BonusTimes	 IsBigWin	 DoubleFree	 	 
 Client To Server	 Bonus Game 領取 	 3003	 CurrID	 	 	 		 		 	 	 	 	 
 Server To Client	 Bonus Game 領取回傳	 3004	 Status	 Rate	 BonusWinMoney	 BonusTimes		 		 	 	 	 	 
 Client To Server	 取得機台資訊	 3005	 CurrID	 	 	 		 		 	 	 	 	 
 Server To Client	 取得機台資訊回傳	 3006	 FreeStatus	 FreeTimes	 BonusStatus	 BonusTimes	 IsBigWin	 BigWinMoney	 Icon x 15	 	 	 
 	 	 	 	 	 	 	 	 	 	 	 	 
 金鑽列車	 	 	 	 	 	 	 	 	 	 	 	 
 Client To Server	 鑽石列車下注	 3101	 CurrID	 OneLineMoney	 GMFreeIconCount	 GMHaveBigWin	 	 	 	 	 	 
 Server To Client	 鑽石列車下注回傳	 3102	 Status	 WinMoney	 NowMoney	 Icon x 15	 FreeStatus	 FreeTimes	 FreeRate	 IsBigWin	 DoubleFree	 
 Client To Server	 鑽石列車取得機台資訊	 3103	 CurrID	 	 	 	 	 	 	 	 	 
 Server To Client	 鑽石列車取得機台資訊回傳	 3104	 FreeStatus	 FreeTimes	 IsBigWin	 BigWinMoney	 Icon x 15	 	 	 	 	 
 劉備傳	 	 	 	 	 	 		 			 	
 Client To Server	 劉備傳下注	 3201	 CurrID	 OneLineMoney	 GMFreeIconCount	 GMHaveBigWin		 			 	
 Server To Client	 劉備傳下注回傳	 3202	 Status	 WinMoney	 NowMoney	 Icon x 15	 FreeStatus	 FreeTimes	 FreeRate	 IsBigWin	 FreeSet	 DoubleFree
 Client To Server	 劉備傳取得機台資訊	 3203	 CurrID	 	 	 		 			 	
 Server To Client	 劉備傳取得機台資訊回傳	 3204	 FreeStatus	 FreeTimes	 IsBigWin	 BigWinMoney	 FreeSet	 FreeRate	 Icon x 15		 	
 Client To Server	 選擇將軍	 3205	 CurrID	 	 	 		 			 	
 Server To Client	 選擇將軍回傳	 3206	 FreeRate	 Odds x 2	 	 		 			 	
 Client To Server	 選擇包子	 3207	 CurrID	 	 	 		 			 	
 Server To Client	 選擇包子回傳	 3208	 Views	 FreeTimes	 Views x 4	 		 			 	
 	 	 	 	 	 	 		 			 	
 小瑪莉	 	 	 	 	 	 		 			 	
 Client To Server	 小瑪莉下注	 3301	 CurrID	 BetMoney x 8	 GMIndexSit	 		 			 	
 Server To Client	 小瑪莉下注回傳	 3302	 Json字串	 	 	 		 			 	
 Client To Server	 送出得分	 3303	 CurrID	 	 	 		 			 	
 Server To Client	 送出得分回傳	 3304	 Json字串	 	 	 		 			 	
 Client To Server	 小瑪莉比大小	 3305	 CurrID	 IsBig	 	 		 			 	
 Server To Client	 小瑪莉比大小回傳	 3306	 Json字串	 	 	 		 			 	
 Client To Server	 小瑪莉抽彩金	 3307	 CurrID	 	 	 		 			 	
 Server To Client	 小瑪莉抽彩金回傳	 3308	 Json字串	 	 	 		 			 	
 Client To Server	 小瑪莉取得機台資訊	 3309	 CurrID	 	 	 		 			 	
 Server To Client	 小瑪莉取得機台資訊回傳	 3310	 Json字串	 	 	 		 			 	
 	 	 	 	 	 	 		 			 	
 水果盤	 	 	 	 	 	 		 			 	
 Client To Server	 水果盤下注	 3401	 	 	 	 		 			 	
 Server To Client	 水果盤下注回傳	 3402	 	 	 	 		 			 	
 Client To Server	 水果盤抽彩金	 3403	 	 	 	 		 			 	
 Server To Client	 水果盤抽彩金回傳	 3404	 	 	 	 		 			 	
 Client To Server	 水果盤取得機台資訊	 3405	 	 	 	 		 			 	
 Server To Client	 水果盤取得機台資訊回傳	 3406	 	 	 	 		 			 	
 	 	 	 	 	 	 		 			 	
 跑馬燈	 	 	 	 	 	 		 			 	
 Client To Server	 取得跑馬燈	 4001	 CurrID	 	 	 		 			 	
 Server To Client	 取得跑馬燈回傳	 4002	 Json字串	 	 	 		 			 	
 好友系統	 	 	 	 	 	 		 			 	
 Client To Server	 取得好有列表	 4101	 CurrID	 	 	 		 			 	
 Server To Client	 取得好有列表回傳	 4102	 Json字串	 	 	 		 			 	
 Client To Server	 取得好友邀請列表	 4103	 CurrID	 	 	 		 			 	
 Server To Client	 取得好友邀請列表回傳	 4104	 Json字串	 	 	 		 			 	
 Client To Server	 邀請好友	 4105	 CurrID	 FindUID	 	 		 			 	
 Server To Client	 邀請好友回傳	 4106	 Json字串	 	 	 		 			 	
 Client To Server	 邀請好友回覆	 4107	 CurrID	 FriendUID	 FriendCID	 IsAccept		 			 	
 Server To Client	 邀請好友回覆回傳	 4108	 Json字串	 	 	 		 			 	
 Client To Server	 刪除好友	 4109	 CurrID	 FriendUID	 FriendCID	 		 			 	
 Server To Client	 刪除好友回傳	 4110	 Json字串	 	 	 		 			 	
 Client To Server	 取得相關數量	 4111	 CurrID	 	 	 		 			 	
 Server To Client	 取得相關數量回傳	 4112	 Json字串	 	 	 		 			 	
 Client To Server	 設定已讀取	 4113	 CurrID	 FriendUID	 FriendCID	 		 			 	
 Server To Client	 設定已讀取回傳	 4114	 Json字串	 	 	 		 			 	
 Client To Server	 取得黑名單列表	 4115	 CurrID	 	 	 		 			 	
 Server To Client	 取得黑名單列表回傳	 4116	 Json字串	 	 	 		 			 	
 Client To Server	 加入黑名單	 4117	 CurrID	 FriendUID	 	 		 			 	
 Server To Client	 加入黑名單回傳	 4118	 Json字串	 	 	 		 			 	
 Client To Server	 刪除黑名單	 4119	 CurrID	 FriendUID	 FriendCID	 		 			 	
 Server To Client	 刪除黑名單回傳	 4120	 Json字串	 	 	 		 			 	
 Client To Server	 設定邀請全部已讀取	 4121	 CurrID	 	 	 		 			 	
 Server To Client	 設定邀請全部已讀取回傳	 4122	 Json字串	 	 	 		 			 	
 	 	 	 	 	 	 		 			 	
 系統公告	 	 	 	 	 	 		 			 	
 Client To Server	 取得系統公告列表	 4309	 CurrID	 	 	 		 			 	
 Server To Client	 取得系統公告列表回傳	 4310	 Json字串	 	 	 		 			 	
 	 	 	 	 	 	 		 			 	
 遊戲設定	 	 	 	 	 	 		 			 	
 Client To Server	 取得遊戲設定	 4301	 CurrID	 	 	 		 			 	
 Server To Client	 取得遊戲設定回傳	 4302	 Json字串	 	 	 		 			 	
 Client To Server	 設定遊戲設定	 4303	 CurrID	 SetIsPushOpen	 SetIsSoundOpen	 SetIsMusicOpen		 			 	
 Server To Client	 設定遊戲設定回傳	 4304	 Json字串	 	 	 		 			 	
 Client To Server	 設定交易認證碼	 4305	 CurrID	 ExchangeCode	 ExchangeCode2	 		 			 	
 Server To Client	 設定交易認證碼回傳	 4306	 Json字串	 	 	 		 			 	
 Client To Server	 更改交易認證碼	 4307	 CurrID	 OldExchangeCode	 NewExchangeCode	 New2ExchangeCode		 			 	
 Server To Client	 更改交易認證碼回傳	 4308	 Json字串	 	 	 		 			 	
 Client To Server	 金流兌換	 4309	 UID	 OrderId	 RecProductId	 		 			 	
 Server To Client	 金流兌換回傳	 4310	 ErrorIndex 	 	 	 		 			 	
 交易系統	 	 	 	 	 	 		 			 	
 Client To Server	 確認交易認證碼	 4401	 CurrID	 CheckExchangeCode	 	 		 			 	
 Server To Client	 確認交易認證碼回傳	 4402	 Json字串	 	 	 		 			 	
 Client To Server	 送出交易	 4403	 CurrID	 CheckExchangeCode	 TargetUID	 TargetCID	 Money	 			 	
 Server To Client	 送出交易回傳	 4404	 Json字串	 	 	 		 			 	
 Client To Server	 領取交易	 4405	 CurrID	 CheckExchangeCode	 TargetUID	 TargetCID	 MesgCurrID	 			 	
 Server To Client	 領取交易回傳	 4406	 Json字串	 	 	 		 			 	
 Client To Server	 取消交易	 4407	 CurrID	 CheckExchangeCode	 TargetUID	 TargetCID	 MesgCurrID	 			 	
 Server To Client	 取消交易回傳 
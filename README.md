# SentimentAnalysisTweetBot  
@UserName キーワード 数 (detail)  
と入力されたとき、キーワードを含むツイートから指定された数のツイートを収集します。  
その後、ツイートを感情分析し、その結果をリプライにツイートします。  
detailを書いた場合、分析の内訳をツイート  
書かれなかった場合、detailを書いた際のstrong_negativeを「アンチかも」としてツイート  
します。  
この判定は現時点では感覚です。    
いい方法があれば改善したい。  

英語に変更してからの感情分析なのであまり信頼性はないので参考程度にしてください  

実行方法  
myStreamListener = SentimentAnalysisTweetBot(consumerKey, consumerSecret, accessToken, accessTokenSecret)  
myStreamListener.filter(track=[account])  

@HeiwaSaverが動いてます

### 多模態 AI 模型 Chameleon
- 同時輸入和輸出文字與圖片，並能將其交錯呈現，這是目前其他模型較少具備的功能。
    
- 雖然參數較少，但在文字相關任務的表現卻能與更大規模的模型相媲美，展現了「早期融合」策略的優勢。
    
- 未來 AI 發展將朝整合更多模態 (影片、音訊、動作、3D) 邁進，最終可能創造出能同時理解和產生多種模態資料的 AI agent，甚至可能引發社會結構的重大改變，例如全民高收入社會的出現。

[[Transformer]]

##### 多模態模型發展經歷三個階段

1. 兩個模型協作
	Bard兩個模型分別處理不同模態
	一個電腦視覺模型先進行image captioning，再把caption加進prompt裏面

2. 兩個模型融合
- 一開始的GPT4-V
- 還是兩個模型在處理，但是是黏在一起處理
    - 一個vision encoder（CLIP）先把圖片處理成含有豐富語義的向量
    - 經過一個projection layer，把這個向量project到跟文字向量的同一個vector space，同一 semantic space
- Pros：主要的模型大腦（transformer layer）會學會同時處理文字跟圖片
- Cons：兩個模型還是分開train的，只是合在一起fine tuning

3. 現在的模型—Eraly-fusion
	大幅提升模型效能和多模態理解能力
- 一開始訓練的時候就用text跟image interleaved 的文章訓練，而且兩個模態都tokenize到同一個token space
- 優點：
    - 模型最一開始就是全部的模態一起學習，不同模態之間能夠學的最好
    - 可以output多模態！！（interleaved） #蛤
    - 不同模態直接會有加成效果
- 缺點：訓練的一些困難（可能就是爲什麽GPT4o只單純output Audio，使出版本只output text），需要很好的資料

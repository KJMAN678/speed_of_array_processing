pandas(DataFrame)、numpy(nddaray)、tensor(GPUなし/あり)でどのくらい処理スピードが異なるのかを比較。  

[ECサイトのデータセット](https://raw.githubusercontent.com/guipsamora/pandas_exercises/master/07_Visualization/Online_Retail/Online_Retail.csv)を加工して使用。  

環境はGoogle Colab、GPUは Tesla T4、条件統一のため型はすべてfloat64とし、tensor化にはpytorchを使用しています。  

Google Colabは[こちら](https://colab.research.google.com/drive/1vKdyL58A9qiF-pNb0FwZ9dFzhrUn0kTn?usp=sharing)。  

### 処理時間の比較

|      |pandas|numpy|tensor(GPUなし)|tensor(GPUあり)|
| ---- | ---- | ---- | ---- | ---- |
|処理時間|約118秒|約149秒|約162秒|約13秒|
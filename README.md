# kaggle-Predicting-Stellar-Class
## 目的
天体を物理的・光学的特性から分類する。
1. 恒星
2. 銀河
3. クエーサー（銀河の中心核）

## 評価指標
Balanced Accuracy

<table class="tg"><thead>
  <tr>
    <th class="tg-0lax" colspan="2" rowspan="2"></th>
    <th class="tg-0lax" colspan="2">予測値</th>
  </tr>
  <tr>
    <th class="tg-0lax">0</th>
    <th class="tg-0lax">1</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0lax" rowspan="2">実測値</td>
    <td class="tg-0lax">0</td>
    <td class="tg-0lax">True Negative (TN)</td>
    <td class="tg-0lax">False Positive (FP)</td>
  </tr>
  <tr>
    <td class="tg-0lax">1</td>
    <td class="tg-0lax">False Negative (FN)</td>
    <td class="tg-0lax">True Positive (TP)</td>
  </tr>
</tbody>
</table>

Balanced Accuracyとは、正例と負例でそれぞれ正答率を出したあとで、その平均を取る。  
$`Balanced Accuracy = (TP/(TP+FN)+TF/(TF+FP))`$


## データ構造

|変数名|説明|
|---|---|
|alpha|赤経（J2000暦）|
|delta|赤緯角（J2000暦）|
|u|紫外線フィルター|
|g|緑色光フィルター|
|r|赤色光フィルター|
|i|近赤外線フィルター|
|z|赤外線フィルター|
|redshift|波長の増加に基づく赤方偏移値|
|spectral_type|銀河系・星のスペクトル分類|
|galaxy_population|銀河群の種類？|


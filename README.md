# 石造物LOD

[石造物3Dアーカイブ](https://stonework-3d-archive.github.io/)で石造物の構造化データを[ウィキデータ](https://www.wikidata.org/)に入力する際に使用するプロパティについて説明します。

### 主な情報
| プロパティ | 説明 | 値の例 | 備考 |
| --- | --- | --- | --- |
| P31(分類) | 石造物の種類 | Q11486001(庚申塔)<br/>Q11516104(月待塔)<br/>Q65643555(地神塔)<br/>Q22812402(道標)<br/>など | 複数入力可 |
| P170(作者) | 石工 | | 不明な場合はQ4233718(作者不明) |
| P186(材料) | 材料 | Q22731(石)、Q484924(凝灰岩)など | 部分毎に異なる場合は、修飾子P518(あてはまる部分)で該当箇所を示す |
| P825(献呈先) | 主尊・祭神 | Q11662826(青面金剛)<br/>Q11446712(如意輪観音)<br/>Q604687(地蔵菩薩)<br/>など | 文字塔でも刻像塔でも可 |
| P1684(銘) | 銘文 | |修飾子P518(あてはまる部分)で刻まれた位置を示す（Q12014132(台座)、Q68345460(前面)、Q14565199(右)、Q13196750(左)、Q68345931(背面)など）<br/>修飾子P3831(オブジェクトの役割)で役割を示す（Q11591100(祭神)、Q3406134(設立日)、Q319608(住所)、Q22812402(道標)など） |

### 刻像に関する情報
| プロパティ | 説明 | 値の例 | 備考 |
| --- | --- | --- | --- |
| P180(題材) | 彫られている像 |Q11662826(青面金剛)<br/>Q11446712(如意輪観音)<br/>Q604687(地蔵菩薩)<br/>など | 修飾子P6022(表情、しぐさ、ポーズ)で像容を示す（Q1986098(立っている)、Q1839786(合掌)など）<br/>修飾子P1114(数)で数を示す（三猿、二鶏など）|
| P2079(制作技法) |  | Q14562306(浅浮き彫り)<br/>Q2520013(丸彫り)など | |

### 所在地に関する情報
| プロパティ | 説明 | 値の例 | 備考 |
| --- | --- | --- | --- |
| P17(国) | 所在する国 | Q17(日本) | |
| P131(位置する行政区画) | 所在する市町村 | Q210628(町田市)<br/>Q1203373(緑区)<br/>など | 緑区のように同名のものが複数ある場合に注意 |
| P625(位置座標) | 所在する緯度経度 | | |

### 造立年に関する情報
| プロパティ | 説明 | 値の例 | 備考 |
| --- | --- | --- | --- |
| P571(設立) | 造立年月日 | | |
| P2348(時代) | 元号 | Q1325001(元禄)<br/>Q1193862(万延)<br/>など | |
* 紀年銘で月日の代わりに季節が刻まれている場合は、修飾子P4241(該当時期)を用いて、Q40720559(春（北半球）)、Q40720564(夏（北半球）)、Q40720568(秋（北半球）)、Q40720553(冬（北半球）)のいずれかを使用する

### サイズに関する情報
| プロパティ | 説明 | 値の例 | 備考 |
| --- | --- | --- | --- |
| P2048(全高) | 高さ |
| P2049(全幅) | 幅 |
| P2610(厚さ) | 厚さ | | 板碑のように奥行の小さいもので使用 |
| P5524(奥行) | 奥行 | | |
* 部分毎のサイズの場合は、修飾子P518(あてはまる部分)で該当箇所を示す

### リンクに関する情報
| プロパティ | 説明 | 値の例 | 備考 |
| --- | --- | --- | --- |
| P18(画像) | Commonsにある画像 | | |
| P4896(3Dモデル) | Commonsにある3Dモデル | | |
| P973(詳細情報URL) | 市町村の文化財解説ページなどへのリンク | | 修飾子でP1476(題名)とP813(閲覧日)を入力 |


------------------------------------------------------------------------------------
# 5/9水
## やったこと  
- mediaとrankingがごっちゃになっていたので切り分けた  
  
## 学んだこと  
- 見た目が同じでも用途が違う場合はクラスを分ける。（ソースコードだけで見て構造が理解できるかセルフチェックしてみる）  
  
## 時間    
- 1:00  
  
------------------------------------------------------------------------------------
# 5/10木
  
## やったこと  
- rankingの修正  
- 画像下出典テキストのレイアウト調整：1:00  
- [wip]twitter下のアイコン：0:40  
- [wip]詳細情報のdlタグのレイアウト：0:30    
  
## 学んだこと・気づいたこと  
- 特に高さ指定を指定なくても、変に高さが出る時はline-heightの値に気をつける  
- インライン要素もdisplay:flexを使うことで綺麗に高さを揃えることができる（display:table-cellでも可能だが今回はflexを採用）（今までline-hight頼りだった）
- どうやってやるか漠然と調べている間に時間が経過している  
  
## 時間  
- rankingの修正：0:40  
- 画像下出典テキストのレイアウト調整：1:00  
- twitter下のアイコン：0:40  
- 詳細情報のdlタグのレイアウト：0:30  
  
------------------------------------------------------------------------------------  
  
# 5/11金
## やったこと  
- コメント部分の修正：0:15
  - （font-sizeの部分対応漏れありましたすみません！）  
- 詳細情報のdlタグのレイアウトの実装：1:10  
- section-container moduleの修正：1:00    
- 合計：2:35  
  
## できなかったこと  
- twitterパーツのクラス名ブラッシュアップ
  
## 学んだこと・気づいたこと  
- dd要素はブロック要素  
- dt、ddタグはhtml5.2からdivでラップすることができる様になった  
- インライン要素にmarginは聞かない  
- 「text-align」は段落に対してのみ有効（インライン要素だと思っていた）  
- z-indexを親要素（ul）につけたが効かなかった。子要素（li）を指定したら動いた。要検証  
    
- 調べながら修正すると１パーツ１時間程度かかる  
- テキストの色を変更したい箇所はたくさんあるが「text-glay（見た目を表しているのでNG）」以外の方法で上手に使い回す方法が見つけられていない  
- 調べごとをする際に「何を知りたいのか」明確にして、それ以外の部分は無視することで無駄な時間を削減できた  
    
------------------------------------------------------------------------------------    
  
# 5/12土
  
## やったこと  
- smacssについてのドキュメントを読み漁る  
- 様々なサイトの構成を分析する  
    
## 時間
- ドキュメント読む：2:00  
- 構成分析：2:00  
  
## 学んだこと・気づいたこと  
  
### base  
- baseはサイト全体の要素のデフォルトスタイル。IDやクラスは使わない。  
- cssのリセットもbaseに含まれる。  
    
### module  
- moduleは再利用可能なパーツ  
- moduelはlayout内に配置される。  
- extend を別モジュールで利用しない。  
- モジュール全部にクラス付ける必要はない。再利用されるときにタグが変更される可能性が無いか考えると良い  
    
### layout  
    
### state  
- stateの命名は「is-」  
- stateはjavascriptに依存する  
    
### その他  
- cssは右から左に評価される  
  - body div.hoge p {}の場合  
　   - 1.ページ内のすべての要素に対してpであるか確認  
　   - 2.pだとしたら、hogeクラスが付与されたdivをdomの最上部へ向かって探す  
　   - 3.div.hogeを見つけたら、bodyを探す  
    
 ------------------------------------------------------------------------------------    
   
# 5/13日
## やったこと  
- text-description修正
- footer修正
- sns修正
- header修正
- mainVisual修正
- media修正
- label修正
- tweet修正
- sectionContainer修正
- paganation修正
- [wip]detail修正中
- BEMについて調べる
- OOCSSについて調べる
   
## 時間
- 12時間

## 学んだこと・気づいたこと
- BEMはシングルクラスでの実装をする。block__element--modifire。この考え方がクラス名を決める時や設計を考える際にとても役に立った。
- OOCSSはマルチクラスでの実装。構造と見た目を分ける。コンテナとコンテンツを切り離す。という考え方がそのままSMACSSに流用できる為、OOCSSで組まれているサイトを探して参考にすることができた。
- 構造：width,height,border,padding,margin
- 見た目：color,border-color,background-colorなど
- インライン要素のインデントには気をつける。
  - <p><span><span/><spam></span></p>これをブロック要素のようにインデントすると1つ目のspanの後に空白が挿入される。
- hoge > * ：子要素を全て選択
- htmlの構造に左右されないのがmoduleと考えることでlayoutとmoduleの切り方の感覚を休み前よりは掴めた（気がする）
  
------------------------------------------------------------------------------------  
   
# 5/14日 火  

## やったこと  
- sectionContainer名前修正
- heading修正
- detail修正
  - さらなるmoduleの切り出し
- anchorの部分の修正
- writerの修正
  
## 時間
- 4時間
  
## 学んだこと・気づいたこと・疑問に思ったこと
- text + iconをflexのaligin-items:centerで行なっているが、他の方法でもできそう（古いブラウザ対策のため）
- cssでの文字省略「text-overflow: ellipsis;」の使い方をまだ理解できていない
- 平日でも詰めれば4時間作業できる

------------------------------------------------------------------------------------  
　
 # 5/15日 水  

## やったこと  
- l-label修正
- border module切り出し
- dlをdetailパーツにした

  
## 時間
- 1時間
  
## 学んだこと・気づいたこと・疑問に思ったこと

- 記事部分とnavi部分は別のコンテナ（article-container nav-container）のように切り分けた方が良いかもしれない（デザインのパターンが微妙に違う）

------------------------------------------------------------------------------------  
  
 # 5/16日 木  

## やったこと  
- anchorBlock→textBlock：名前修正
- borderBottom→border-bottom：名前修正
- balloon内のmediaのtext overflow:ellipsisを使ったテキストの省略最適化
- l-labelの子要素セレクタ指定修正
- iconのデフォルトカラー設定
- facebookのアイコン色違うの修正
- スタイル調整
  
## 時間
- 3時間30分
  
## 学んだこと・気づいたこと・疑問に思ったこと
  
### text-overflow-ellipsisを使ったテキストの省略について
- ブロック要素に指定しないと動かない
- 複数のインライン要素をラップしてるブロック要素に対しては無効
- 横幅を指定する必要があるが、white-space: nowrap;で改行が無効になる為、横並びコンテナ内で使用したい場合はwidth:100%から横に並んでいるコンテンツの幅を引いてあげないと要素からはみ出る
  
### background-containとは
- 要素に対して、背景画像全体が表示されるように調整されます
- cover:縦方向に画像が拡大される。横は切れる
- auto:特に画像サイズは変わらずそのまま表示される
- (便利な参考：http://keicode.com/script/css-background-size.php)

### viwport vh,vw,vmax,vmin,%について
- vmax,はvh,vwの大きい方の値を使う
- %とviewportの違いは%は親要素から相対的に計算されるのに対して、viewportは画面の幅から相対的に計算される
- 計算式は xxpx/画面サイズ = xxx(%)
- 欠点はソースを見たときに分かりにくい
- （便利なツール：https://codepen.io/netsi1964/full/NyzmeQ）

------------------------------------------------------------------------------------  
  
# 5/17日 金  

## やったこと  

### 学んだこと・気づいたこと・疑問に思ったこと
- ios6以降は日本フォントのデフォルトが明朝体になっているのでゴシック体を使いたい場合、sans-serifの指定が必須。
- スマホの最小フォントサイズは8px。12px以下は使わないのが無難
- androidデバイスで使える共通フォント「Doroid sans」「Roboto」の２つ
- androidの日本語フォントはデバイスごとにバラバラ。表示できる日本語フォントは1フォントのみ
- androidの標準ブラウザはfont-family意味無し

- 便利な一覧：https://mw-s.jp/2017css-font-win-mac/
- （便利な参考：https://saruwakakun.com/font-family）



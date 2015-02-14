-----------------------------------
#Androidアプリのプログラムに挑戦  
画像の表示
-----------------------------------

![09](https://github.com/miyake-yasunaga/03_Image/blob/master/images/09.png)

文字の表示はなんとなくわかりました。  
では、今度は画像をを表示させてみましょう。  

まずはテキストの追加と同じようにＧＵＩで画像のウィジェットを追加します。  

Projectのファイル一覧から｢activity_main.xml｣を選択して  
中央下に表示されてる  

｢Design｣のタブをクリックしてＧＵＩ画面を表示します。  

｢Widgets｣の下の方にある｢ImageView｣を選択した状態で  
右のAndroid画面にマウスを移動させて適当な場所でクリックします。  

![01](https://github.com/miyake-yasunaga/03_Image/blob/master/images/01.png)


中央下に表示されてる  
｢Text｣のタブをクリックしてソース画面を表示します。  

imageウィジェットの記述が追加されています。  

![02](https://github.com/miyake-yasunaga/03_Image/blob/master/images/02.png)


次に画像が保存されているフォルダから表示したいファイルを選択して  
app\src\res\drawableの下にドラッグアンドドロップします  

(※あまり大きな画像を選択すると、実行した時にメモリ不足でエラーとなります。  
とりあえずはお試しで100KB程度の画像を選んでください。）  

![03](https://github.com/miyake-yasunaga/03_Image/blob/master/images/03.png)

そのままドラッグアンドドロップすると移動(MOVE)になります。  
コピーしたい場合は、Ctlを押しながらドラッグアンドドロップすればいいようです。  

![04](https://github.com/miyake-yasunaga/03_Image/blob/master/images/04.png)

app\src\res\drawableの下にimages01.jpgが追加されました。  
まだこれだけでは、まだ画面イメージに画像は表示されません。  

![05](https://github.com/miyake-yasunaga/03_Image/blob/master/images/05.png)


activiti_Main.xmlのImageViewのタグに  
先ほどコピペしたファイルを画像ソースとして指定します。  

           android:src="@drawable/image01"  
（途中まで入力すると候補が出てくるのでファイル名を選択します。）  

![06](https://github.com/miyake-yasunaga/03_Image/blob/master/images/06.png)

これで右側の画面イメージに画像が表示されました。  
画像とボタンが重なってしまっているので  
ちょっと体裁を整えたほうがいいですね。  

![07](https://github.com/miyake-yasunaga/03_Image/blob/master/images/07.png)

ボタンの位置をimageViewの下に修正してやりましょう。  

android:layout_below="@+id/imageView"  

これでいい感じに表示できました！！  

![08](https://github.com/miyake-yasunaga/03_Image/blob/master/images/08.png)

ビルドしてみます。  

![09](https://github.com/miyake-yasunaga/03_Image/blob/master/images/09.png)


次回はテキストと同じように  
ボタンで画像を切り替えてみましょう。  


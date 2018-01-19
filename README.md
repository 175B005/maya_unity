# maya_unity
MayaとUnityの相互関係
- [maya unity](https://youtu.be/0awywk4IqRU)

- [FBX Exporter](http://u3d.as/XWD)

1. unity起動
1. 上記のExporterをimport
1. unity で変更したい基本モデルを作成  
ここで作成したモデルが当たり判定にもなっているので、大きさはある程度あわせておく、（変更は後から可能。）
1. Exportしたいモデルを入れたフォルダを作成（フォルダを固定したほうがいい。）
1. Editのproject setting < EBX Exportが追加されているので、それを選択。
1. ![](https://raw.githubusercontent.com/175B005/maya_unity/master/Description1.jpg)
1. Export　Path先ほど作成したファイルを選択
1. 自分のPC上に入っているMayaのバージョンを選択(2016からUnityとの連携機能入ってる？？)
1. Install Unity Integrationを選択→自分の今のプロジェクトが選択されているので、  
そのままOK。（ Run Component Undaterは情報をアップデートする機能、更新。）
1. 勝手にこれでMayaが起動します。↓ここからMayaでの設定。
1. Mayaが起動したら、Window < 設定/プリファレンス <　プリファレンス < 設定　< リニア；→メートルに変更  Saveします。
1. ![](https://raw.githubusercontent.com/175B005/maya_unity/master/Description3.jpg)
(MayaとUnityではスケールの単位が違うため、Unityにあわせる為、Unityがメートルなので、あわせる目的があります。)
1. Unityに戻ります。
1. Mayaで変更したい基本モデル（先ほど作成したもの）を選択し、右クリックでメニューを表示
1. 下にExport Model...とConvert To Linked Instanceが追加されているので  
Convert To Linked Instanceのほうを選択します。  
1. ![](https://raw.githubusercontent.com/175B005/maya_unity/master/Description2.jpg)
すると勝手にリンク用のプレファブが生成されます。（先ほど作成したフォルダ）
1. その後さっきのExport Modelを選択して、先ほどと同じファイルを選択（そのままでOKのはず、、）
1. Exportが完了したらMaya側に行って、今度はimportします。  
1. ![](https://raw.githubusercontent.com/175B005/maya_unity/master/Description4.jpg)
ファイル　< Unity < import (unity でExportした場所からFBXファイルを選択（unityで作った変更したいモデル）)
1. mayaの中心にモデルが表示されます。
1. maya上で変更を加えて、Export（ファイル　< Unity < Export）する。
1. unityに戻ると勝手に更新され、テクスチャやモデルの形状など連携ができている。

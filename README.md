# MagnifyAPI_test
PowerShellからMagnifyAPIで拡大鏡を制御するスクリプトです。    
vbsはコンソールを立ち上げずに実行するためのもので、本体はps1ファイルです。  
名前付きパイプ経由で終了シグナルを受け取ると拡大状態が解除され縮小されます。  
**拡大するとzoomout.ps1を実行するかプロセスを止めるか再起動しないと元に戻りません。**

### INFINITAS (2023/02/09)
* JoyToKeyでE3とE4をvbsスクリプトに割り当てることによって演奏レーンに合わせて拡大縮小できます。
  - これ以外にもファンクションキーやWindowsキーに絡むショートカットキーが殆どほとんど使えないという制約を回避して実行する方法が存在し、尚且別窓が立ち上がらなければ好きなタイミングで拡大縮小できると思います。
* 2P側の場合はMagSetFullscreenTransform関数の2番目の引数を書き換えてください。
* Now Loading画面で判定位置を初期化するので必ず拡大した状態で起動してください。
  - 拡大していないと裏で流れている曲とキー音がズレます。
  - Now Loading画面の後は一旦縮小したり演奏前に拡大するなどして問題ないです。
* 120FPSに対応している環境の場合は拡大しても120FPSのままプレーできます。
  - ASUS VG258Q(1280x720)で確認

### 注意
このスクリプトを使用することによって生じる問題等の責任を一切負いません

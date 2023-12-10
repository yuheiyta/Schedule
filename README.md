# Schedule
.DRGファイルがGUI上で作成できる。
SKDTools.py -- CUIで.DRGファイルを作成することができるモジュール
SKED_GUITool.py -- GUIで.DRGファイルを作成することができるプログラム。SKDTools.pyのfunctionを使用している。

## Install (anaconda環境)
anacondaで仮想環境を作り、そこで動かす方法（pythonやモジュールのバージョン等が散らからない（仮想環境で閉じる）のでおすすめ）  

anacondaのインストールは[こちら](https://www.anaconda.com/download)  
必要なパッケージは conda_requirements.txt に記載してある。  
conda_requirements.txt のヘッダーに書いてあるように、`$ conda create --name <env> --file conda_requirements.txt` で仮想環境を作ると必要なパッケージがインストールされる。  
\<env> は環境名。例えばschedule。  
環境を構築したら、 `$ conda activate <env>` で環境に入る。  
本プログラムを実行するための適当なディレクトリを作成し、SKDTools.py, SKED_GUITool.py, antenna.sch を置く。  
作成したディレクトリで （もしくはpathを通すなどして） `python SKED_GUITool.py` とすると起動する。  
antenna.sch はJVNのwebサイトなどから最新版を取得して使用すると良い。なお本ページのantenna.sch は、使用頻度が低いアンテナをコメントアウトしてある。

（以下は必要に応じて）  
.skdファイルを作成したい時は、drgconv2020.out の実行ファイルを同じディレクトリに置く必要がある。  
相関用.xmlファイルを作成したいときは、mk_skd.py（穐本さん作成）を同じディレクトリに置く必要がある。

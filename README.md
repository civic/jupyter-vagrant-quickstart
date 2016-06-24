jupyter vagrant環境構築クイックスタート
===============================

anacondaでjupyterをインストールする。

インストール
------------

```
$ vagrant up
```

実行開始
----------

```
$ vagrant ssh -c "anaconda3/bin/jupyter notebook --no-browser --notebook-dir=/vagrant --ip=0.0.0.0"
```

ホストマシンのブラウザからlocalhost:8888で開く。


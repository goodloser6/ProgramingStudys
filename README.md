# ProgramingStudys

１　SSH Keyの作成
ssh-keygen -t rsa -b 4096 -C "your_email@example.com"
※示された場所にそのまま保存（Enterキーを押す）
※パスワードを確認用と２度同じものを入力
※処理後の画面をキャプチャで残しておこう

２　SSH Keyの内容をクリップボードにコピー
clip < ~/.ssh/id_rsa.pub
※.sshの位置は先ほどSSH Keyが保存された場所

３　Githubにログインする

４　ページ右上の自分のアカウントアイコンをクリックし、出てきたメニューから「Setting」をクリックする

５　左メニュー内から「SSH and GPG keys」ボタンをクリックし、「New SSH Key」ボタン（緑）をクリックする

６　「SSH keys / Add new」というページが表示される

７　Title欄に識別子を入力
※何でもよいので、"ProgramingStudysSSH"のようなわかりやすい名前をつけておこう

８　Key欄に先ほどid_rsa.pubからコピーした内容を貼り付ける
※もし、途中でコピー内容が変わってしまった場合は、Ctrl + Vで過去のコピーから参照するか、もしくは再度「clip < ~/.ssh/id_rsa.pub」でコピーしてくる

９　「Add SSH Key」ボタン（緑）をクリックする

１０　鍵マークがついたSSH Keyが作成されていることを確認する

１１　git clone git@github.com:fukuda0330/ProgramingStudys.git

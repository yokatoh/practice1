
# practice1
何度かやって、
$ git push -u origin main
がようやくうまくいった。
pushしたら、githubのサーバからパスワードを聞かれて、入れたらようやくつながった。pushできた。
（GitHubサーバが、Authentication Succeeded　　となった）


<必要だった準備らしき行為、確証はない>

・ssh-keygen　が効いたか？

・user.emailにGit Hubに登録したアドレスを設定したからアカウントは聞かれなかった？



# practice2
ローカルのファイルを消してしまったらうまくいかなくなった

以下で何とか元に戻す（M365 Copilot恐るべし）

>git reset --hard origin



# practice3
4月からのorganization移行に関して

M356 Copilotに聞くと方法を教えてくれた
「gitでorganizationをまたいで、リポジトリをコピーする方法を教えて」

方法1：git clone → 新しいOrganizationにpush
方法2:通常のclone＋remote追加
方法3：GitHubの「Fork」機能


# practice4
再度このファイルを更新してpushするにはcommitからでいいのか？確認する
なんかうまくいかんからやりなおし（foo.txtの変更でおかしくなった
add →　commit　→　push　でうまくいく
編集したらaddからやり直し、を忘れないようにしないといけない

# practice5
pullrequest してみる

>git checkout -b pullreq

 git add → git commit → git push

ithub のサイトでプルリクする
　どのブランチからどのブランチにマージするかをボタンで選択した上で、「Pull request」のタブを触る
　「Compare & pull request」のボタンを押す　（これでプルリク発行）
　そこに書いてあるので、コメント入れたりして、承認するとサーバ上のmainにマージされる

# practice6
bash にemacsをいれる　Windows側でASMRとか設定 した

起動するにもwinpty emacs -nw　としないといけないみたい

恐ろしいことに、cmd でもemacsが起動する。パスはC:\msys64\usr\bin


# practice7
windows 用のemacs　を git bashから起動できるようにする
ttyの問題とかなくなってC-cが使えて便利


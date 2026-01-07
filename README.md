# practice1
何度かやって、
>git push -u origin main
がようやくうまくいった。
push前に、githubのサーバからパスワードを聞かれて、入れたらようやくつながった。pushできた。
（GitHubサーバが、Authentication Succeeded　　となった）


<必要だった準備らしき行為、確証はない>
・ssh-kegen　が効いたか？
・user.emailにGit Hubに登録したアドレスを設定したからアカウントは聞かれなかった？



#practice2
ローカルのファイルを消してしまったらうまくいかなくなった

以下で何とか元に戻す（M365 Copilot恐るべし）

>git reset --hard origin



#practice3
4月からのorganization移行に関して

M356 Copilotに聞くと方法を教えてくれた
「gitでorganizationをまたいで、リポジトリをコピーする方法を教えて」

方法1：git clone → 新しいOrganizationにpush
方法2:通常のclone＋remote追加
方法3：GitHubの「Fork」機能


#practice4
再度このファイルを更新してpushするにはcommitからでいいのか？確認する


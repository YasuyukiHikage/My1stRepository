# My1stRepository

接続テスト用リポジトリ

Windowsでgit cloneなどを実行した時に下記のエラーが表示される
```
fatal: unable to access 'https://github.com/Username/RepositoryName.git/': SSL certificate problem: unable to get local issuer certificate
```

Unable to resolve "unable to get local issuer certificate" using git on Windows with self-signed certificate
https://stackoverflow.com/questions/23885449/unable-to-resolve-unable-to-get-local-issuer-certificate-using-git-on-windows


```
git config --global http.sslbackend schannel
```

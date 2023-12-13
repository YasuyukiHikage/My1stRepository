# My1stRepository

接続テスト用リポジトリ

## Windowsでgit cloneなどを実行した時に下記のエラーが表示される
```
fatal: unable to access 'https://github.com/Username/RepositoryName.git/': SSL certificate problem: unable to get local issuer certificate
```

Unable to resolve "unable to get local issuer certificate" using git on Windows with self-signed certificate
https://stackoverflow.com/questions/23885449/unable-to-resolve-unable-to-get-local-issuer-certificate-using-git-on-windows

→下記コマンドを実行する
```
git config --global http.sslbackend schannel
```

## git pushを行った時に下記のエラーが発生する

```
remote: Permission to YasuyukiHikage/My1stRepository.git denied to YasuyukiHikage.
fatal: unable to access 'https://github.com/YasuyukiHikage/My1stRepository.git/': The requested URL returned error: 403
```

→資格情報マネージャーからgh:github.comの情報を削除後、もう一度pushする

HTTPS接続を用いたGitHubへのpush時に403エラーが出た時の対処法
https://scrapbox.io/Mijinko/HTTPS%E6%8E%A5%E7%B6%9A%E3%82%92%E7%94%A8%E3%81%84%E3%81%9FGitHub%E3%81%B8%E3%81%AEpush%E6%99%82%E3%81%AB403%E3%82%A8%E3%83%A9%E3%83%BC%E3%81%8C%E5%87%BA%E3%81%9F%E6%99%82%E3%81%AE%E5%AF%BE%E5%87%A6%E6%B3%95
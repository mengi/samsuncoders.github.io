# samsuncoders.github.io

samsuncoders.org websitesi kaynak kodları

Topluluğa katılmak için bu repoyu forkladıktan sonra kendi bilgisayarınıza klonlayarak **source** branchında `data/topluluk.yml` dosyasına kendinizi ekleyin.

Örnek:

```bash
git clone git@github.com:kullaniciadi/samsuncoders.github.io && cd samsuncoders.github.io
git checkout source

vim data/topluluk.yml
```

Örnek kullanıcı:

```yaml
users:
  - kullaniciadi:
    name: Adiniz Soyadiniz
    title: Unvaniniz
    company: Sirket
    email: "email@adresi.com"
    website: "http://website.com"
    social:
      github: "https://github.com/kullaniciadi"
      twitter: "https://twitter.com/kullaniciadi"
      linkedin: "https://linkedin.com/in/kullaniciadi"

      # facebook, google vb de ekleyebilirsiniz.
```

Örnek build:

```bash
bundle install

# gemler kurulduktan sonra test etmek icin
middleman s
# http://localhost:4567

# toplulukta kendizi gordukten sonra kendi forkunuzda deploy
middleman deploy # yapmasaniz da olur

# merge edilecek branch source branchidir
# o yuzden source branchini commitlemelisiniz
git add .
git commit -m 'Yeni user kullaniciadi'
git push origin source
```

Pull request açmak için reponuzdan pull requests sekmesine giderek new pull request butonuna tıklayabilirsiniz.

Eğer kimseyi topluluktan silmediyseniz merge edilecektir.

İlginiz için teşekkürler :smiley:

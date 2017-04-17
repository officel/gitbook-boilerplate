# toc

目次

<!-- toc -->

## h2-1

ページ中に目次を追加するプラグイン

## h2-2

book.json の plugins に toc を追加

### h3-1

ページ中に`<!-- toc -->`を追加

### h3-2

book.json の pluginsConfig に設定を入れておくとhtmlのclassが追加される

#### h4

```book.json
{
    "plugins": ["toc"],
    "pluginsConfig": {
        "toc": {
            "addClass": true,
            "className": "toc"
        }
    }
}
```

##### h5

ページ内目次が必要な場合に使う

###### h6

長いページには便利だけど、h5とh6にはつかないみたい

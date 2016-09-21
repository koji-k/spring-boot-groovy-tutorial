# Hello world

適当なディレクトリに移動して、`hello.groovy`を作成し、中身を以下のようにしてください。  

```groovy
@RestController
class WebApplication {

    @RequestMapping("/")
    String home() {
        "Hello World!(Groovy version : ${GroovySystem.version})"
    }
}
```

できたら、以下のコマンドを実行してください。  

```
spring run hello.groovy
```

初回起動時は依存ライブラリなどが **自動で** ダウンロード、設定されるので時間がかかります。  
しばらくすると`Tomcat started on port(s): 8080 (http)`という表示されます。  
では実際にブラウザで[http://localhost:8080/](http://localhost:8080/)にアクセスしてください。  
画面に **Hello World!(Groovy version : 2.4.7)** と表示されることが確認できると思います。  
Groovyインストールしてないぞ！？と思った方も居るかも知れませんが、SpringBootによって自動的にインストール、設定されたものです。  
つまり、Groovyを態々自分でインストールする必要はありません。  

SpringBootとGroovyの力を利用すれば、ビルドツールすら必要としないWEBアプリケーションを開発することが出来ます。  
当然大きなアプリケーションになればビルドツールを導入したほうが色々便利なのですが、まずはこのシンプルさを利用して軽快に、そして楽しくSpringBootとGroovyでWEBアプリケーションを開発していきましょう。

*以降誠意作成中！*
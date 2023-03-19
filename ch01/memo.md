# 学習メモ:Ruby 入門
## 1.Ruby言語の基本概念と構文
### Rubyの歴史、特徴、用途
・Rubyとは
Runyとは、1995年にまつもと ゆきひろさんが公開したプログラミング言語です。

・特徴

・用途

### Rubyのインストール方法
・Rubyの開発環境構築
Macでは、デフォルトでインストールされている

.RUbyのインストール確認
```sh
$ ruby -v
```

・test.rbファイルの実行
```sh
$ ruby test.rb
```
### コメントの書き方
```ruby
# puts "Hello World"
```


### 出力方法（puts, print, p）
・出力方法
```ruby
puts "Hello World" # 改行される
puts 'Hello World' # 改行される

print "Hello World" # 改行されない
p "Hello World" # putsの省略形
```


## 2.データ型（数値、文字列、シンボル、配列、ハッシュ）と変数
### 変数の宣言と代入
変数の宣言と代入
```ruby
name = "tanaka"
puts name # 出力結果:tanaka
name = "yamada"
puts name # 出力結果:yamada
```

変数展開
```ruby
name ="田中"
puts "私の名前は、#{name}です" #シングルクォーテーションは、不可
```
### 数値、文字列、シンボルの操作


### 配列、ハッシュの生成と操作
```ruby
name = ["山田","田中","佐藤"]
puts name
# 出力結果:
# 山田
# 田中
# 佐藤

puts name[0] # 出力結果:山田
```

```ruby
name = ["山田","田中","佐藤"]
puts name
# 出力結果:
# 山田
# 田中
# 佐藤

puts name[0] # 出力結果:山田
```

ハッシュ
```ruby
user = {"name" => "namaka" , "age" => 20}
puts user
# 出力結果:{"name"=>"namaka", "age"=>20}
puts user["name"]
# 出力結果:namaka
```

ハッシュのキーにシンボルを使用
```ruby
user = {:name => "namaka" , :age => 20}
puts user
# 出力結果:{:name=>"namaka", :age=>20}
puts user[:name]
# 出力結果:namaka
```

ハッシュの省略
```ruby
user = {name: "namaka" , age: 20}
puts user
# 出力結果:{:name=>"namaka", :age=>20}
puts user[:name]
# 出力結果:namaka
```


配列
```ruby
users = [
    {name: "namaka" , age: 20},
    {name: "yamada" , age: 25}
]
puts users
# 出力結果:
# {:name=>"namaka", :age=>20}
# {:name=>"yamada", :age=>25}
puts users[0]
# 出力結果:{:name=>"namaka", :age=>20}
puts namaka
# 出力結果:namaka
```

## 3.演算子と式（算術演算子、比較演算子、論理演算子）
### 算術演算子（加算、減算、乗算、除算、剰余、べき乗）
数字の計算
```ruby
puts 2+3 # 出力結果:5
puts 3+2 # 出力結果:1
puts 2*3 # 出力結果:6
puts 4/2 # 出力結果:2
puts 5%3 # 出力結果:2
```

変数の計算
```ruby
x = x + 1
x = x - 1
x = x * 1
x = x / 1
x = x % 1
```

変数の計算（省略）
```ruby
x += 1 # x = x + 1
x -= 1 # x = x - 1
x *= 1 # x = x * 1
x /= 1 # x = x / 1
x %= 1 # x = x % 1
```

### 比較演算子（等価、非等価、大小比較）


### 論理演算子（AND、OR、NOT）

## 4.条件分岐（if文、case文）(2時間)
### if文、elsif、elseの使い方
条件分岐
age = 30
```ruby
if age > 20
    puts "20歳より上です"
end

puts a < b # aがb未満ならtrue
puts a <= b # aがb以下ならtrue
puts a > b #　aがbより大きいならtrue
puts a >= b # aがb以上ならtrue
puts a == b # aとbが同じならtrue
puts a != b # aとbが違うならtrue
```
### unless文
```ruby
```

### case文を使った条件分岐
```ruby
```

## 5.繰り返し処理（each, for, while, until）
### eachを使った繰り返し
```ruby
配列.each do |変数名|

end
```

### for文
```ruby
```

### while文、until文
```ruby
```

### 繰り返しの制御（break, next, redo）

```ruby
```

## 6.メソッドの定義と呼び出し
### メソッドの定義方法
```ruby
```

### 引数と戻り値
```ruby
```

### メソッドの呼び出し方法
```ruby
```

### ブロックとイールド
```ruby
```

## 7.クラスとオブジェクト指向プログラミング
### クラスの定義
```ruby
```


### インスタンス変数とアクセサメソッド
```ruby
```

### インスタンスメソッド
```ruby
```

### 継承、オーバーライド、スーパー

## 8.モジュールとミックスイン
### モジュールの定義

### モジュールのインクルード

### 名前空間

## 9.例外処理
### 例外の種類

### begin、rescue、ensure
```ruby
```

```ruby
```

### 例外の発生と捕捉

## 10.ファイル入出力
### ファイルのオープンとクローズ

### ファイルからの読み込み

### ファイルへの書き込み

## 11.RubyGemsとライブラリの利用
### RubyGemsの概要

### インストールされているGemの確認

### Gemのインストールとアンインストール

### Gemを使ったプログラムの作成


## 12.コードの品質向上（リファクタリング、テスト）
### リファクタリングの概念と目的

### リファクタリングの基本的な手法（変数名の改善、メソッドの抽出、コードの簡略化）

### テストの概要と目的

### テストフレームワーク（RSpecやMinitest）の導入

### 単体テストの作成と実行

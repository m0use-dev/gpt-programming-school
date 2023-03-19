# 学習メモ:Ruby 入門

## 1.Ruby 言語の基本概念と構文

### Ruby の歴史、特徴、用途

・Ruby とは
Runy とは、1995 年にまつもと ゆきひろさんが公開したプログラミング言語です。

・特徴

・用途

### Ruby のインストール方法

・Ruby の開発環境構築
Mac では、デフォルトでインストールされている

.RUby のインストール確認

```sh
$ ruby -v
```

・test.rb ファイルの実行

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

## 4.条件分岐（if 文、case 文）(2 時間)

### if 文、elsif、else の使い方

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

### unless 文

```ruby

```

### case 文を使った条件分岐

```ruby

```

## 5.繰り返し処理（each, for, while, until）

### each を使った繰り返し

```ruby
配列.each do |変数名|

end
```

### for 文

```ruby
for num in 1..5 do
  puts num
end
# 出力結果:
# 1
# 2
# 3
# 4
# 5
```

### while 文、until 文

```ruby

```

### 繰り返しの制御（break, next, redo）

```ruby

```

## 6.メソッドの定義と呼び出し

### メソッドの定義方法
メソッドの定義
```ruby
def hello
  "Hello!"
end
```

### 引数と戻り値

```ruby
def 
end
```

### メソッドの呼び出し方法

```ruby
# メソッドの定義
def greet(name)
  "Hello, #{name}!"
end

# メソッドの呼び出し
puts greet("田中")  #=> "Hello, 田中!"
puts greet("山田")    #=> "Hello, 山田!"
```

### ブロックとイールド

```ruby

```

## 7.クラスとオブジェクト指向プログラミング

### クラスの定義

クラスの定義

```ruby
class クラス名
end

class User

end
```

インスタンス変数

```ruby
class User
  attr_accessor :name
  attr_accessor :age
	def info
    return "name:#{self.name} age:#{self.age}"
  end
end
user1 = User.new
user1.name = "田中"
user1.price = 20
puts user11.info
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

## 11.RubyGems とライブラリの利用

### RubyGems の概要

RubyGems.org
https://rubygems.org 

### インストールされている Gem の確認
インストールされている Gem の確認
```sh
$ gem list --local
```

### Gem のインストールとアンインストール
Gem のインストール
```sh
$ gem install 〇〇〇
$ gem install bundler
```
Gem のアンインストール
```sh
$ gem uninstall 〇〇〇
$ gem uninstall bundler
```

### Gem を使ったプログラムの作成

## 12.コードの品質向上（リファクタリング、テスト）

### リファクタリングの概念と目的

### リファクタリングの基本的な手法（変数名の改善、メソッドの抽出、コードの簡略化）

### テストの概要と目的

### テストフレームワーク（RSpec や Minitest）の導入

### 単体テストの作成と実行





ターミナルから入力

```
name = gets.chomp
number = gets.chomp.to_i
```

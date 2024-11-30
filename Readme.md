This is readme!
let's create a small browser.
this browser is seem to be made from Rust.

Memo

# Part1

## 前提を整理する
レンダリングツリー：ブラウザ内部での中間表現  
Web IDL：Web ブラウザが提供している、JavaScript エンジンに対するインターフェイス。DOM API や Fetch API がその例。  
IDL (Interface Definition Language)：プログラミング言語に依存しない言語。異なるプログラムやコンポーネント間で通信を行うためのインターフェースを定義するために使用される。  
Binding：JavaScript と Web ブラウザ側実装を繋げるコード。その一部は、Web IDL をもとに生成されている。  


画面生成の過程  
![alt text](image.png)  

JSが介入する場合  
![alt text](image-1.png)

## HTML を取り扱う
パース処理：HTML 文字列を DOM のようなツリーに変換する処理  
クレート：Rustプログラミング言語におけるコードのパッケージ（モジュール化された単位）  
EBNF (Extended Backus-Naur Form) ：コンピュータ言語やデータ形式の文法を記述するための形式的な記法の一つ。文法規則を簡潔かつ柔軟に記述するために使われます。  
to_string() ： &str から String を生成する。Rustには&strとStringという型が存在する。データの保存領域が違うっぽいよくわからず。 


HTMLからDOMが生成される  
![alt text](image-2.png)

EBNF (Extended Backus-Naur Form)   
![alt text](image-3.png)
![alt text](image-4.png)

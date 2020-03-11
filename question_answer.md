「もしtrueであれば、以下の処理を実行する」に少し補足させていただきます。

>if trueは、何がtrueの時に実行されるのか

if trueの条件式ですが、if文の前に書いた変数が関わっており
「もし変数に関する条件式がtureであれば、以下の処理を実行する」
となります。

例題の場合
「ageに関する条件式がtureであれば、以下の処理を実行する」
となるため下記が実行されます。

（age = 18 の場合は、age < 20 がtrue）

[test.rb]
```
age = 18

if age < 20
  puts "あなたは未成年です(1)"
end

if true
  puts "あなたは未成年です(2)"
end
```
結果
```
$ ruby test.rb
あなたは未成年です(1)
あなたは未成年です(2)
```

git push origin master

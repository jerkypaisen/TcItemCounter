# TcItemCounter
You can count the specified item in TC.
（TCの中の特定のアイテムを集計します。）

# How to use
1.Please enter the item shortname you want to aggregate in the configuration file.
（最初にコンフィグファイルに集計したいアイテムのショート名を指定してください。）

ShortName List
https://www.corrosionhour.com/rust-items-database/


2.Open the F1 console and enter a "tic" command. only be executed by an administrator.
（F1コンソールを開いて、ticコマンドを入力してください。実行できるのは管理者のみです。）



# Commands
This plugin provides F1 console commands using the syntax.

Aggregate specific items in TC for each owner of TC.
When you specify a number in the command argument, the names are displayed as many times as the specified number. 
```
tic [num]
```

Aggregate specific items in TC for each team leader.
When you specify a number in the command argument, the names are displayed as many times as the specified number. 
```
ttic [num]
```

# Configuration
The settings and options can be configured in the TcItemCounter.json file under the config directory. The use of an editor and validator is recommended to avoid formatting issues and syntax errors.

format
```
{
  "count targets": {
    "Item short name": base point number
  }
}
```

exp format
```
{
  "count targets": {
    "dogtagneutral": 1,
    "bluedogtags": 10
  }
}
```

※base point numberで指定した数字が、アイテム集計時に個数に掛け算されます。

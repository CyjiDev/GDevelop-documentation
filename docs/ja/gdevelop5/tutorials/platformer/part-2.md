---
title: プラットフォーマー チュートリアル Part 2：プレイヤーキャラクターを作ろう
---
# プラットフォーマー チュートリアル Part 2：プレイヤーキャラクターを作ろう

今回はプレイヤーキャラクターの作り方を説明します。

次の内容を含んでいます。

- プレイヤーキャラクターを表示するオブジェクトを作成する
- 矢印キーでオブジェクトを操作できるようにする
- カメラにプレイヤーキャラクターを追いかけさせる

## シリーズ

いま読んでいるのは[プラットフォーマー チュートリアル](/ja/gdevelop5/tutorials/platformer)の **Part 2** です。

1. [プラットフォーマー チュートリアル Part 1](/ja/gdevelop5/tutorials/platformer)
2. プラットフォーマー チュートリアル Part 2
3. [プラットフォーマー チュートリアル Part 3](/ja/gdevelop5/tutorials/platformer/part-3)
4. [プラットフォーマー チュートリアル Part 4](/ja/gdevelop5/tutorials/platformer/part-4)
5. [プラットフォーマー チュートリアル Part 5](/ja/gdevelop5/tutorials/platformer/part-5)
6. [プラットフォーマー チュートリアル Part 6](/ja/gdevelop5/tutorials/platformer/part-6)
7. [プラットフォーマー チュートリアル Part 7](/ja/gdevelop5/tutorials/platformer/part-7)
8. [プラットフォーマー チュートリアル Part 8](/ja/gdevelop5/tutorials/platformer/part-8)

## ステップ 1：オブジェクトを作成する

最初に、プレイヤーキャラクターを表示するオブジェクトを作成します。チュートリアルの Part 1 をお読みになっていれば、手順はもうお分かりでしょう。

プレイヤーキャラクター用のオブジェクトを作成する手順は次の通りです。

1. 「Player」という名前の**スプライト**オブジェクトを作成します。
2. アニメーションの唯一のフレームとして「p1_stand.png」アセットを使います。
3. アニメーションの名前に「Idle」（待機）と入力します。
4. オブジェクトをシーンにドラッグしてインスタンスを配置します。

![](/gdevelop5/tutorials/platformer/player-object.jpg)

!!! note

    キャラクターをアニメーションさせる方法は[プラットフォーマー チュートリアル Part 4](/ja/gdevelop5/tutorials/platformer/part-4) で説明します。

## ステップ 2：オブジェクトにビヘイビアを追加する

ゲームをプレビューすると分かりますが、この「Player」オブジェクトはまだ操作できません。なぜなら、デフォルトのままではオブジェクトは何もしないからです。オブジェクトに何かさせるには、1 つ以上の[ビヘイビア](/ja/gdevelop5/behaviors)を割り当てる必要があります。

GDevelop には数クリックでオブジェクトに追加できるビヘイビアがたくさん付属しています。そのひとつに**プラットフォーマーキャラクター**ビヘイビアがあり、これを使うとオブジェクトをプレイヤーキャラクターとして操作できるようになります。

では以下の手順で**プラットフォーマーキャラクター**ビヘイビアをオブジェクトに追加しましょう。

1. オブジェクトパネル上で **Player** オブジェクトを右クリックします。
2. **オブジェクトを編集**を選択します。
3. **ビヘイビア**タブに切り替えます。
4. **オブジェクトにビヘイビアを追加**をクリックします。
5. **プラットフォーマーキャラクター**を選択します。
6. **適用**をクリックします。

ゲームをプレビューすると、矢印キーでキャラクターを操作できるはずです。ただし、これには副作用があります。**プラットフォーマーキャラクター**ビヘイビアは重力の影響を受けるため、今の状態ではプレイヤーキャラクターがあっという間にフレームから落ちていってしまいます。

![](/gdevelop5/tutorials/platformer/platformer-character-behavior-preview.gif)

## ステップ 3：カメラにオブジェクトを追いかけさせる

キャラクターがフレームから落ちるのを防ぐために、プラットフォーム（足場）が必要です。それから、プレイヤーを追いかけるカメラも。[チュートリアルの次の章](/gdevelop5/tutorials/platformer/part-3)では、プラットフォームを作ります。なので、ここではカメラを作りましょう。

プレイヤーを追いかけるカメラの作成には、[イベント](/ja/gdevelop5/events)を使います。GDevelop のイベントには、原因と結果を定義できます。すなわち、何かが起きると（原因）別の何かが引き起こされる（結果）ように設定するのです。

イベントは 2 つの部分から構成されます。条件とアクションです。条件はイベントがいつ実行されるかを定義し、アクションはイベントが実行されると何が起きるのかを定義します。

GDevelop は、ゲームに必要と思われるあらゆる種類の条件とアクションを取り揃えています。ここで利用できる選択肢を把握することが、GDevelop を使いこなす上で重要な位置を占めています。今回の場合で言うと、このゲームには**オブジェクトの中央にカメラを合わせる**というアクションがぴったりです。

**オブジェクトの中央にカメラを合わせる**アクションを追加する手順は、次の通りです。

1. イベントエディターを開きます。
2. **新しいイベントを追加**をクリックします。
3. 条件を指定せずに、**アクションを追加**をクリックします。条件を指定しないと、アクションは無条件に毎フレーム実行されます。したがって、ゲームが毎秒 60 フレームで実行されたなら、アクションも毎秒 60 回実行されます。
4. **その他のアクション**をクリックします。
5. **レイヤーとカメラ**を展開します。
6. **オブジェクトの中央にカメラを合わせる**を選択します。
7. 「Player」オブジェクトを選択します。
8. **OK**をクリックします。

![](/gdevelop5/tutorials/platformer/center-camera-event.jpg)

ゲームをプレビューすると、キャラクターはやっぱり落下するでしょう。プラットフォームがまだありませんから。でもカメラは、キャラクターを追いかけ続けるはずです。その結果、今度はキャラクターが画面から消えることはありません。

![](/gdevelop5/tutorials/platformer/center-camera-on-object-preview.gif)

## 次のステップ

次は[プラットフォーマー チュートリアル Part 3](/ja/gdevelop5/tutorials/platformer/part-3) で、お待ちしています。
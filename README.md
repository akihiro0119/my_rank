## Usersテーブル

| Column               | Type    | Options      |
|--------------------  |------------------------|
| username             | string  | null: false  |
| email                | string  | null: false  |
| password 　　　　　　  | string  | null: false  |
| password_confirmation| string  | null: false  |
| profile              | text    |              |
| profile_image_id     |         |              |

### Association

- has_many :posts



## postsテーブル

| Column               | Type        | Options                       |
|--------------------  |---------------------------------------------|
| title                | string      | null: false                   |
| body                 | text        | null: false                   |
| image                |             |                               |
| user_id　　　　　　    | references  | null: false foreign_key:true  |


### Association

- belongs_to :user

### ５W1H

- WHAT　
個人的ランキング投稿アプリ

- WHY
年末年始で様々なランキング番組があるが、「自分はこう思う！」と思った時に
細かい好みの差が出ていると感じた。その好みの差が上辺だけでない本当に趣味嗜好の近い人に巡り会えるヒントになると思った。
ネガティブなニュースが多い今の世の中や、自己主張がしづらい人が多い日本人にはポジティブで自分をもっと主張できる場所が必要なのではないかと感じた。

- WHO 
年末年始のランキング番組をもっと楽しみたい人に
今年一年の出来事やなど、思い出を語りたい人

- HOW
画像と文字数300文字以内で投稿してもらう
コメント機能を実装して繋がりやすくする
いいね機能やタグなどを付けて分かりやすくする（追加実装）  - WHEN　　WHERE どこでも インターネット環境さえあれば

###　使い方使用例

・好きなアーティストの好きな曲ランキング ・今年あった衝撃的な出来事ランキング
・気に入ってる地元の景色ランキング

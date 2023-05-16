# chat-gpt-website-sample-dentist-appointment-list

## 歯医者さんの予約システムの予約一覧確認画面

### 🔻 プロンプト( フリーバージョンなのでこのくらい言わないときちんと作ってくれない )
<pre>
歯医者さんの予約システムの予約一覧確認画面を作成してください
- bootstrap を使用
- スマホで見る場合、TABLE が横スクロールするようにする為、TABLE の親要素の DIV の class 属性に table-responsive を使用
- TD 内の文字列やコンテンツが改行しないように TD要素に対して white-space: nowrap を style 要素内で指定する
</pre>

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <style>
    td {
      white-space: nowrap;
    }
  </style>
  <title>予約一覧</title>
</head>

<body>
  <div class="container mt-5">
    <h2>予約一覧</h2>
    <div class="table-responsive">
      <table class="table">
        <thead>
          <tr>
            <th>予約日時</th>
            <th>患者名</th>
            <th>電話番号</th>
            <th>操作</th>
          </tr>
        </thead>
        <tbody>
          <tr>
            <td>2023-05-17 10:00</td>
            <td>山田太郎</td>
            <td>090-1234-5678</td>
            <td>
              <button class="btn btn-primary">編集</button>
              <button class="btn btn-danger">キャンセル</button>
            </td>
          </tr>
          <tr>
            <td>2023-05-18 14:30</td>
            <td>鈴木花子</td>
            <td>080-9876-5432</td>
            <td>
              <button class="btn btn-primary">編集</button>
              <button class="btn btn-danger">キャンセル</button>
            </td>
          </tr>
          <!-- 他の予約情報も同様に追加 -->
        </tbody>
      </table>
    </div>
  </div>
</body>

</html>
```

### [リアルタイム HTML に貼り付けて、『新しく開く』](https://toolbox.winofsql.jp/html-page.php)

![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/91754615-32e5-4c71-9a7b-c5480343b393)

- スマホ表示

  ![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/8dd57f8c-c94b-4b4c-a849-35900c2b2b27)
 
  ![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/82ba02e0-f735-4e8a-a7df-0439b94df768)


## 歯医者さんの予約システムの予約登録画面

### 🔻 プロンプト
<pre>
歯医者さんの予約システムの予約登録画面を作成してください
- bootstrap を使用
- ヘッダ部にサイトの各ページへ画面遷移するリンクを作成
</pre>

```html
<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/css/bootstrap.min.css">
  <title>予約登録</title>
</head>

<body>
  <nav class="navbar navbar-expand-lg navbar-dark bg-dark">
    <div class="container">
      <a class="navbar-brand" href="#">歯医者さんの予約システム</a>
      <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNav"
        aria-controls="navbarNav" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNav">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a class="nav-link" href="#">予約一覧</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">患者管理</a>
          </li>
          <li class="nav-item">
            <a class="nav-link" href="#">設定</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>

  <div class="container mt-5">
    <h2>予約登録</h2>
    <form>
      <div class="form-group">
        <label for="date">予約日</label>
        <input type="date" class="form-control" id="date" name="date" required>
      </div>
      <div class="form-group">
        <label for="time">予約時間</label>
        <input type="time" class="form-control" id="time" name="time" required>
      </div>
      <div class="form-group">
        <label for="name">患者名</label>
        <input type="text" class="form-control" id="name" name="name" required>
      </div>
      <div class="form-group">
        <label for="phone">電話番号</label>
        <input type="tel" class="form-control" id="phone" name="phone" required>
      </div>
      <button type="submit" class="btn btn-primary">登録</button>
    </form>
  </div>

  <script src="https://code.jquery.com/jquery-3.5.1.slim.min.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.5.3/dist/umd/popper.min.js"></script>
  <script src="https://stackpath.bootstrapcdn.com/bootstrap/4.5.2/js/bootstrap.min.js"></script>
</body>

</html>
```

### [リアルタイム HTML に貼り付けて、『新しく開く』](https://toolbox.winofsql.jp/html-page.php)

![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/90bae651-5529-4bc3-b12a-08d6a82f09f0)

- スマホ表示

  ![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/12b7a8a9-c2ee-484c-b07e-e563f8830e46)

  ![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/c2299323-565f-463a-9913-0a7f88067bb9)

  ![image](https://github.com/winofsql/chat-gpt-website-sample-dentist-appointment-list/assets/1501327/c5754476-ece0-4538-8e3f-6ae8de468e85)

- ### ChatGPT による補足説明

ヘッダ部にはBootstrapの`navbar`コンポーネントを使用して作成しました。`navbar-brand`クラスを使用してロゴやサイト名を表示し、`navbar-toggler`クラスを使用してモバイル表示時のメニューの切り替えを行います。各ページへのリンクは`navbar-nav`クラスを持つリストとして配置し、`nav-link`クラスを使用してスタイリングしています。

予約登録フォームは`container`クラス内に配置されています。`form-group`クラスを使用して各入力項目をグループ化し、`form-control`クラスを持つ`input`要素を使用して入力フィールドを作成しています。登録ボタンは`btn`クラスと`btn-primary`クラスを使用してスタイリングしています。

最後に、Bootstrapに必要なJavaScriptの依存関係を読み込んでいます。jQuery、Popper.js、BootstrapのJavaScriptファイルを順に読み込むことで、Bootstrapの機能を有効化しています。

以上が歯医者さんの予約システムの予約登録画面の例です。適宜、リンクのURLやフォームの入力項目をカスタマイズしてください。

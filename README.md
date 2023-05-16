# chat-gpt-website-sample-dentist-appointment-list

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



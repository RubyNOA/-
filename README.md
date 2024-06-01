<!DOCTYPE html>
<html lang="ja">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>占いサイト</title>
</head>
<body>
    <div class="container">
        <h1>今日の占い</h1>
        <form id="fortuneForm">
            <label for="name">名前：</label>
            <input type="text" id="name" name="name" required>
            <button type="submit">占う</button>
        </form>
        <div id="result"></div>
    </div>
    <script>
        document.getElementById('fortuneForm').addEventListener('submit', function(event) {
            git add index.html
git commit -m "Initial commit"
git push origin main
            
            event.preventDefault();
            const name = document.getElementById('name').value;
            const resultDiv = document.getElementById('result');
            resultDiv.innerHTML = `<p>${name}さん、今日の運勢は...</p>`;
        });
    </script>
</body>
</html>
-

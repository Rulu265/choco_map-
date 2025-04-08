# choco_map-
<!DOCTYPE html>
<html lang="ja">
<head>
  <meta charset="UTF-8">
  <title>全国チョコレート販売店MAP</title>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/css/bootstrap.min.css">
</head>
<body class="bg-light">
  <div class="container py-4">
    <h1 class="mb-4 text-center">🍫 全国チョコレート販売店MAP 🍫</h1>
    <div class="row row-cols-1 row-cols-md-2 g-4">
      {% for shop in shops %}
      <div class="col">
        <div class="card shadow-sm">
          <div class="card-body">
            <h5 class="card-title">{{ shop.name }}</h5>
            <p class="card-text">{{ shop.prefecture }} - {{ shop.address }}</p>
            <p class="card-text text-muted">{{ shop.description }}</p>
          </div>
        </div>
      </div>
      {% endfor %}
    </div>
  </div>
</body>
</html>

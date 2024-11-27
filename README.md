<!doctype html>
<html lang="fr">
  <html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="/static/style.css">
    <title>bestof</title>
</head>
<body>
    <h1>bestof</h1>
  <h2>by sosga</h2>
    <form action="/" method="get">
        <input type="text" name="query" placeholder="Enter search term">
        <input type="submit" value="Search">
    </form>
    {% if results %}
        <h2>Results:</h2>
        <ul>
        {% for url, content in results %}
            <li><a href="{{ url }}">{{ url }}</a></li>
        {% endfor %}
        </ul>
    {% endif %}
</body>
</html>

<!DOCTYPE html>
<html>
<head>
    <title>Text Summarizer</title>
</head>
<body>
    <h2>Summarize Your Notes</h2>
    <form action="/summarize" method="post">
        <textarea name="text" rows="10" cols="60" placeholder="Paste your text here..."></textarea><br><br>
        <button type="submit">Summarize</button>
    </form>

    {% if summary %}
        <h3>Summary:</h3>
        <p>{{ summary }}</p>
    {% endif %}
</body>
</html>

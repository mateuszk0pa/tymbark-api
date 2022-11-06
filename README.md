<!DOCTYPE html>
<html lang="pl">
<head>
    <meta charset="UTF-8">
    <meta name="author" content="Mateusz Kopaszewski">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Docs - Tymbark API</title>
    <link rel="stylesheet" href="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.6.0/styles/monokai.min.css">
    <script src="//cdnjs.cloudflare.com/ajax/libs/highlight.js/11.6.0/highlight.min.js"></script>
    <script>hljs.highlightAll();</script>
    <style>
        body {
            background-color: #272822;
        }
        section {
            margin-left: 25%;
            margin-right: 25%;
            margin-top: 2%;
            color: white;
            background-color: gray;
            border-radius: 20px;
        }
        .text {
            margin-left: 4%;
            margin-right: 4%;
        }

        @media (max-width: 899px) {
            section {
                margin-left: 13%;
                margin-right: 13%;
                margin-top: 7%;
                color: white;
                background-color: gray;
                border-radius: 20px;
            }
            img {
                width: 80%;
            }
        }
    </style>
</head>
<body>
  <section>
      <br>
    <div class="text">
      <h1 class="title">Tymbark API</h1>
      <a href="https://github.com/mateuszk0pa"><img src="https://img.shields.io/badge/Created%20by:-mateuszk0pa-success?style=for-the-badge&logo=github"></a>
      <h3 class="co-to">Co to?</h3>
      <p class="co-to-p">
        Tymbark API to zbiór <b>523</b> haseł z napojów marki Tymbark
      </p>
      <h3>Przykłady użycia:</h3>
      <h4>GET: <pre><code class="language-python">https://tymbark-api.k0pa.repl.co</code></pre></h4>
      <h4>Python:</h4>
      <pre><code class="language-python">import requests
haslo = requests.get("https://tymbark-api.k0pa.repl.co")
haslo = haslo.json()
haselko = haslo['haslo']
numer = haslo['numer']
print(haselko)
print(numer)
      </code></pre>
      <h4>Wynik:</h4>
        <pre><code class="language-python">POBALUJMY
13

Process finished with exit code 0
      </code></pre>


      <h4>Curl:</h4>
      <pre><code class="highlightjs-curl">curl -X GET https://tymbark-api.k0pa.repl.co
      </code></pre>
        <h4>Wynik:</h4>
        <pre><code class="language-python">{"haslo": "FRESHSTYLER", "numer": "130"}
      </code></pre>
    </div>
      <br>
  </section>
</body>
</html>

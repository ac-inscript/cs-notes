<!DOCTYPE html>
<html>
<head>
  <meta charset="UTF-8">
  <title>Epigraphic Record Generator</title>

  <style>
    body { font-family: Times New Roman, sans-serif; max-width: 800px; margin: 20px auto; }
    input, textarea { width: 100%; margin-bottom: 10px; }
    textarea { height: 80px; }
    pre { background: #840c0c; padding: 10px; }
  </style>
</head>

<body>

<h1>Epigraphic Record Generator</h1>

<label>Type of inscription</label>
<input id="type_inscription">

<label>Type of object</label>
<input id="type_object">

<label>Location of creation</label>
<input id="place_creation">

<label>Location of discovery</label>
<input id="place_discovery">

<label>Collection</label>
<input id="collection">

<label>Material</label>
<input id="material">

<label>Writing system</label>
<input id="writing_system">

<button onclick="generate()">Generate record</button>

<h2>Output (Markdown)</h2>
<pre id="output"></pre>

<script>
function generate() {

  let type_inscription = document.getElementById("type_inscription").value;
  let type_object = document.getElementById("type_object").value;
  let place_creation = document.getElementById("place_creation").value;
  let place_discovery = document.getElementById("place_discovery").value;
  let collection = document.getElementById("collection").value;
  let material = document.getElementById("material").value;
  let writing_system = document.getElementById("writing_system").value;

  let result =
`## Epigraphic Record

**Type of inscription:** ${type_inscription}

**Type of object:** ${type_object}

**Place of creation:** ${place_creation}

**Place of discovery:** ${place_discovery}

**Collection:** ${collection}

**Material:** ${material}

**Writing system:** ${writing_system}
`;

  document.getElementById("output").innerText = result;
}
</script>

</body>
</html>
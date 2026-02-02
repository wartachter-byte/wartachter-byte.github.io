<!DOCTYPE html>
<html>
<head>
  <title>Dual-use file</title>
</head>
<body>

# This is Markdown-visible content

This text shows up when viewed as Markdown.

<template id="html-only">
  <h1>HTML-only content</h1>
  <p>This renders ONLY when viewed as HTML.</p>
</template>

<script>
  const tpl = document.getElementById("html-only");
  document.body.appendChild(tpl.content.cloneNode(true));
</script>

</body>
</html>

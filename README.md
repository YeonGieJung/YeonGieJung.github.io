YeonGieJung.github.io
<!doctype html>
<html lang="ko">
  <head>
    <meta charset="utf-8" />
    <title>CSS</title>
    <style type="text/css">
      div {
        margin: 10px 0px;
        text-align: center;
        font-family: Consolas, monospace;
        font-style: italic;
        font-size: 13px;
      }
      .a {
        border: 4px dashed #bcbcbc;
      }
      .b {
        border: thick dotted #f44336;
      }
      .c {
        border: 5pt groove #3f51b5;
      }
      .d {
        border: 0.4em inset #009688;
      }
      .e {
        border: 5px ridge #ff5722;
      }
    </style>
  </head>
  <body>
   
<html lang="ko">
  <head>
    <meta charset="utf-8">
    <title>CSS</title>
		<style>
			input[id="cb1"] + label {
				display: inline-block;
				width: 20px;
				height: 20px;
				border: 2px solid #bcbcbc;
				cursor: pointer;
			}
			input[id="cb1"]:checked + label {
				background-color: #666666;
			}
			input[id="cb1"] {
				display: none;
			}
		</style>
  </head>
  <body>
    <h3>Checkbox</h3>
    <input type="checkbox" id="cb1">
    <label for="cb1"></label>
  </body>
</html>
    <div class="a">
      <p>gray: 4px dashed #bcbcbc;</p>
    </div>
    <div class="b">
      <p>red: thick dotted #f44336;</p>
    </div>
    <div class="c">
      <p>dark blue: 5pt groove #3f51b5;</p>
    </div>
    <div class="d">
      <p>green: 0.4em inset #009688;</p>
    </div>
    <div class="e">
      <p>orange: 5px ridge #ff5722;</p>
    </div>
  </body>
</html>

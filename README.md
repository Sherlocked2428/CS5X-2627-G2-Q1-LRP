# CS5 X Group 2 Learning Resource Package

## Instructions for contribution

(See `template.html` for an example file; you may copy-paste from there to create a new file.)

Write your content in HTML inside the `div` element with ID `content`, with paragraphs within the `p` tag. Note that $\LaTeX$ for math typesetting is supported via MathJax.

Python code is also supported via Skulpt; please follow this format when including Python code snippets.
- Please be sure to change all instances of the `yourcode` and `output` IDs (corresponding to the code snippet and its output, respectively) in order for the IDs of the code snippets to not collide.
- You may edit your code inside the `textarea`; please make sure that the first line of your Python code starts right after the `<textarea>` tag and the last line ends right before the `</textarea>` tag (both without any whitespace between).
- When the user clicks the `Run` button, the output will be displayed inside the `pre` tag. Input (i.e. user input whenever the `input` function is used) is collected using JavaScript alerts.

```html
<!--START CODE--------------------------------------------------------->
<p>
<form> 
<label class="python-label">PYTHON CODE</label>
<textarea id="yourcode" cols="40" rows="10" class="python-code">print("Hello World!")</textarea><br /> 
<button type="button" onclick="runit('yourcode', 'output')">Run</button> 
</form></small>
</p>
<label class="python-label">OUTPUT</label>
<pre id="output" class="code-output"></pre>
<!--END CODE----------------------------------------------------------->
```
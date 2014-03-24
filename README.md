# Markdown Header Numbers
Prepends section numbers to headers starting at header h2.

## Installation
Place the `number_headers.py` script in the extensions folder of the markdown package: `markdown/extensions/`

## Usage

### Command Line

`markdown.py filename.md -x num_header --file=output.html`

### Script

```python
import markdown
import number_headers
myext = number_headers.NumberHeadersExtension(None)

with open('filename.md', 'r') as f:
    text = f.read()

html = markdown.markdown(text, extensions=[myext])
```


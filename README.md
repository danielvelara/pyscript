# PyScript

> Daniel Velázquez Lara A01632646

> Run Python in Your HTML

PyScript is a framework that allows users to create rich Python applications in the browser using HTML's interface and the power of [Pyodide](https://pyodide.org/en/stable/) , [WASM](https://webassembly.org/), and modern web technologies. The PyScript framework provides users at every experience level with access to an expressive, easy-to-learn programming language with countless applications.

- What is PyScript? Well, here are some of the core components:

  - Python in the browser: Enable drop-in content, external file hosting, and application hosting without the reliance on server-side configuration
  - Python ecosystem: Run many popular packages of Python and the scientific stack (such as numpy, pandas, scikit-learn, and more)
  - Python with JavaScript: Bi-directional communication between Python and Javascript objects and namespaces
  - Environment management: Allow users to define what packages and files to include for the page code to run
  - Visual application development: Use readily available curated UI components, such as buttons, containers, text boxes, and more
  - Flexible framework: A flexible framework that can be leveraged to create and share new pluggable and extensible components directly in Python

- _i.e. PyScript is just HTML, only more powerful, thanks to the rich and accessible ecosystem of Python libraries._

---

- To run we can import the WASM Python compiler and start using `<py-script>` to embed python in the browser

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width,initial-scale=1" />

    <title>PyScript Hello World</title>

    <link rel="icon" type="image/png" href="favicon.png" />
    <link rel="stylesheet" href="https://pyscript.net/latest/pyscript.css" />

    <script defer src="https://pyscript.net/latest/pyscript.js"></script>
  </head>

  <body>
    Hello world! <br />
    This is the current date and time, as computed by Python:
    <py-script>
      from datetime import datetime now = datetime.now() now.strftime("%m/%d/%Y,
      %H:%M:%S")
    </py-script>
  </body>
</html>
```

<a href="https://ibb.co/Z2jpzTM"><img src="https://i.ibb.co/g42LZgR/image.png" alt="image" border="0"></a>

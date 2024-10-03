Here is a comprehensive list of **Emmet commands** and **abbreviations** available in **Visual Studio Code (VS Code)**. Emmet is incredibly powerful for writing HTML and CSS code faster, using shorthand syntax to generate code blocks.

### **Basic Tag Expansions**

1. **Single Tags**

   - **`div`** → `<div></div>`
   - **`p`** → `<p></p>`
   - **`a`** → `<a href=""></a>`

2. **Self-closing Tags**
   - **`img`** → `<img src="" alt="">`
   - **`input`** → `<input type="text">`

### **HTML Boilerplate**

- **`html:5`** → Full HTML5 boilerplate.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Document</title>
  </head>
  <body></body>
</html>
```

### **Tag Multiplication**

- **`ul>li*5`** → Creates a list with 5 `<li>` tags.

```html
<ul>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
  <li></li>
</ul>
```

- **Multiplication and Text**  
   `ul>li*3{Item $}` →

  ```html
  <ul>
    <li>Item 1</li>
    <li>Item 2</li>
    <li>Item 3</li>
  </ul>
  ```

- **Numbered Items with Zero Padding**  
   `ul>li.item-$$*3` →
  ```html
  <ul>
    <li class="item-01"></li>
    <li class="item-02"></li>
    <li class="item-03"></li>
  </ul>
  ```

### **Classes and IDs**

- **`div.class`** → `<div class="class"></div>`
- **`div#id`** → `<div id="id"></div>`
- **`div.class1.class2`** → `<div class="class1 class2"></div>`

### **Attributes**

- **`a[href="https://example.com"]`** → `<a href="https://example.com"></a>`
- **`input[type="checkbox"]`** → `<input type="checkbox">`

### **Text inside Tags**

- **`p{Hello World}`** → `<p>Hello World</p>`
- **`h1{Title}`** → `<h1>Title</h1>`

### **Nesting Elements**

- **`nav>ul>li*3`** → Generates nested elements.

```html
<nav>
  <ul>
    <li></li>
    <li></li>
    <li></li>
  </ul>
</nav>
```

### **Sibling Elements**

- **`h1+p+bq`** → Creates sibling elements.

```html
<h1></h1>
<p></p>
<blockquote></blockquote>
```

### **Grouping Elements**

- **`(header>nav>ul>li*3)+footer>p`** → Groups elements together.

```html
<header>
  <nav>
    <ul>
      <li></li>
      <li></li>
      <li></li>
    </ul>
  </nav>
</header>
<footer>
  <p></p>
</footer>
```

### **Numbering Elements**

- **`li.item-$*5`** → Generates 5 list items with numbered classes.

```html
<li class="item-1"></li>
<li class="item-2"></li>
<li class="item-3"></li>
<li class="item-4"></li>
<li class="item-5"></li>
```

### **Repeating Elements with Content**

- **`li.item-$*5{Item $}`** → Generates 5 `<li>` elements with unique content.

```html
<li class="item-1">Item 1</li>
<li class="item-2">Item 2</li>
<li class="item-3">Item 3</li>
<li class="item-4">Item 4</li>
<li class="item-5">Item 5</li>
```

### **Custom Attributes**

- **`a[title="Click here" target="_blank"]`** → Custom attributes in tags.

```html
<a title="Click here" target="_blank"></a>
```

### **CSS Syntax**

1. **Selectors**

   - **`w100`** → `width: 100px;`
   - **`m10`** → `margin: 10px;`
   - **`p10-20`** → `padding: 10px 20px;`

2. **Shortcuts for properties**

   - **`bgc`** → `background-color: ;`
   - **`fz`** → `font-size: ;`
   - **`bd1s`** → `border: 1px solid;`

3. **Multiplication in CSS**

   - **`m10*4`** → `margin: 10px 10px 10px 10px;`

4. **CSS Abbreviations**

   - **`w100p`** → `width: 100%;`
   - **`h50p`** → `height: 50%;`
   - **`bd1s#000`** → `border: 1px solid #000;`

5. **Property Expansion**  
   `m10` → `margin: 10px;`  
   `p10-20` → `padding: 10px 20px;`  
   `w100` → `width: 100px;`  
   `h100` → `height: 100px;`  
   `bgc` → `background-color: ;`

6. **Multiple Properties**  
   `pos:a;top0;left0` →

   ```css
   position: absolute;
   top: 0;
   left: 0;
   ```

7. **Shorthand for Box Model**  
   `m10-20` → `margin: 10px 20px;`  
   `p5-10` → `padding: 5px 10px;`

8. **Shorthand for Colors**  
   `c#0f0` → `color: #0f0;`  
   `bg#000.5` → `background-color: rgba(0,0,0,0.5);`

9. **Flexbox**  
   `d:f` → `display: flex;`  
   `ai:c` → `align-items: center;`  
   `jc:c` → `justify-content: center;`

10. **Positioning**  
    `pos:a` → `position: absolute;`  
    `pos:r` → `position: relative;`

11. **Text Styles**  
    `fs16` → `font-size: 16px;`  
    `fw700` → `font-weight: 700;`  
    `tt:u` → `text-transform: uppercase;`  
    `ta:c` → `text-align: center;`

12. **Border Radius**  
    `brd50%` → `border-radius: 50%;`

### **Commenting Elements**

- **`!`** → Adds a `DOCTYPE` and comments for HTML.

### **Emmet for JSX (React)**

1. **Self-closing tags in JSX**

   - **`div.className`** → In JSX, use `className` instead of `class`.

   ```jsx
   <div className="className"></div>
   ```

2. **Custom JSX Tags**

   - **`MyComponent`** → Creates custom JSX components.

   ```jsx
   <MyComponent></MyComponent>
   ```

3. **Self-closing JSX components**
   - **`MyComponent/`** → Creates a self-closing component.
   ```jsx
   <MyComponent />
   ```

### **Tables**

1. **Simple Table**
   - **`table>tr*2>td*3`** → Creates a table with 2 rows and 3 columns.
   ```html
   <table>
     <tr>
       <td></td>
       <td></td>
       <td></td>
     </tr>
     <tr>
       <td></td>
       <td></td>
       <td></td>
     </tr>
   </table>
   ```

### **Forms**

1. **Basic Form Structure**

   - **`form>label+input[type=text]+button`** → Creates a basic form.

   ```html
   <form>
     <label></label>
     <input type="text" />
     <button></button>
   </form>
   ```

2. **Form with Multiple Inputs**
   - **`form>input[type=text]*3+button`** → Generates a form with 3 text inputs and a button.
   ```html
   <form>
     <input type="text" />
     <input type="text" />
     <input type="text" />
     <button></button>
   </form>
   ```

---

### **Customizing Emmet in VS Code**

You can also customize Emmet settings in VS Code by adding configurations in `settings.json`. For example:

- **Enable Emmet in JSX files**:
  ```json
  "emmet.includeLanguages": {
      "javascript": "javascriptreact",
      "vue-html": "html",
      "razor": "html"
  }
  ```

### Key Emmet Shortcuts in VS Code:

- **Expand Abbreviation**: `Tab` or `Ctrl+E` (Mac: `Cmd+E`)
- **Wrap with Abbreviation**: `Ctrl+Shift+P` (Mac: `Cmd+Shift+P`)
- **Balance (Select HTML Tags)**: `Ctrl+Shift+A` (Mac: `Cmd+Shift+A`)
- **Go to Matching Pair (HTML Tags)**: `Ctrl+Alt+T` (Mac: `Cmd+Option+T`)

---

### **Official Site documentation**

These are the most common and useful Emmet commands for VS Code, covering HTML, CSS, JSX, and more. For more advanced usage, you can check the official [Emmet documentation](https://docs.emmet.io/).

# markdown-tests
a playground to test how github renders certain things in markdown

# jsdoc tutorial links
jsdoc style: {@tutorial basic}

link to generated html: [basic](tutorial-basic.html)

link to source: [basic](basic.md)

# code
`inline single`

```inline triple```

```
block
triple
```

`
block
single
`

# html entities
Entity dec: &#177;

Entity name: &plusmn;

Entity hex: &#xb1;

Raw: ±

# code
```js
window.location.href = '/';
```


# tables with multiple lines of code

#### closest I could get in markdown, results in multiple rows
| Status | Response  |
| ------ | --------- |
| 200    | `json`                          |
|        | `   {`                          |
|        | ` "id": 10,`                    |
|        | ` "username": "alanpartridge",` |
|        | ` more code...`                 |
|        | `}`                             |
| 400    |                                 |

#### with HTML table
<table>
<tr><th>Old</th><th>New</th></tr>
<tr><td>
```js
window.location.href = '/';
```
</td><td>
```js
window.location.assign('/');
```
</td></tr>
</table>

#### with HTML table and HTML pre/code
<table>
<tr><th>Old</th><th>New</th></tr>
<tr><td><pre class="prettyprint source lang-js" lang="js"><code>
window.location.href = '/';
</code></pre></td><td><pre class="prettyprint source lang-js" lang="js"><code>
window.location.assign('/');
</code></pre></td></tr>
</table>

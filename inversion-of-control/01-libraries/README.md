React selbst ist nur eine View Libary,
die uns Logik an die Hand gibt um DOM zu manipulieren.

---

### History Lesson 👀

Bevor wir JS Libraries zum Rendern von UI genutzt haben,
hatten wir nur good old HTML und Javascript zur Verfügung.

Man musste direkt mit den Browser APIs kommunizieren, um
DOM Manipulationen auszuführen.

Bei kleineren Anwendungen ganz ok, bei großen und komplexen
Applikationen aber der absolute Wartungs Horror.

---

### JS Libraries to the Rescue. React 😍

JS Libraries setzen sich über die Browser APIs und kümmern sich um die ganze "harte" Arbeit.

So wird aus `document.createElement` ein `React.createElement` call.

Benutzt React einmal direkt "ohne alles".
Dafür könnt ihr bspw. Unpkg benutzen.

```html
<script src="https://unpkg.com/react@17.0.0/umd/react.development.js"></script>
<script src="https://unpkg.com/react-dom@17.0.0/umd/react-dom.development.js"></script>
```

React ist Platform unabhängig, daher nutzen wir ReactDOM, um React zu sagen,
dass wir hier mit DOM Nodes zu tun haben.

Wir haben jetzt `React`und `ReactDOM` auf unserem globalen `window` object.
Damit können wir bereits React Apps schreiben.

```javascript
React.createElement(type, props, ...children);
```

[📜 React ohne JSX](https://reactjs.org/docs/react-without-jsx.html)

Wir erstellen also React Elemente und
können diese dann am Ende mit der ReactDOM Library renden lassen.

```javascript
ReactDOM.render(reactElement, rootNode);
```

---

### Kombination von Libraries

So schreibt natürlich niemand React.
Was wir wollen und was ihr kennt ist die XML ähnliche Syntax - JSX. Dafür brauchen wir eine "Transformation" bzw. einen Compiler von JSX zu Javascript. Babel hilft uns hier gerne und weil es in JS geschrieben ist, können wir es auch direkt einsetzen im Browser 🤯.

Thank god - Unpkg hat auch hier direkt was parat.

```html
<script src="https://unpkg.com/@babel/standalone@7.12.4/babel.js"></script>
```

Damit wir Babel nutzen können müssen wir nur den script Tag muten indem wir den type auf `text/babel` setzen.

Der Browser interpretiert den JS Code nun nicht mehr, dafür weiß Babel was es zu tun hat, compiliert den Code und packt in die Seite.

### Inversion of Control

Bezugnehmend auf unsere Unterscheidung zwischen Framework und Libraries,
haben wir also immer selber die volle Kontrolle, wann, wie und weshalb etwas ausgeführt wird.

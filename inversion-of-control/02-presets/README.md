So wie in `01-libraries` will natürlich niemand seinen
Code schreiben. Deshalb greifen wir zu Frameworks.
Oder etwa nicht?

---

### Presets

Create React App ist viel mehr ein Preset zu konfigurationen bestimmter Libraries,
als dass es ein Framework ist.

"Under the hood" arbeiten hier Webpack, Babel, Eslint, etc.
Mit einer vorgegebenen Konfiguration, die es euch erlaubt einfach eine `src/index.js` anzulegen
und von dort aus euren React Code zu schreiben, ohne euch um die Konfiguration der anderen
Libraries zu kümmern.

Ihr könnt die Settings auch `ejecten`, dann habt ihr wieder die volle Kontrolle
über die Einstellungen.

Es handelt sich hier also genau genommen nicht um die `Inversion of control`, die wir von einem Framework erwarten.

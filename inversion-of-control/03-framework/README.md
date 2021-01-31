Wenn wir also von einem Framework sprechen,
dann handelt es sich dabei um eine Anwendung, die mit Vorgaben
definiert, wie wir unseren Code schreiben müssen.

Anhand dieser Vorgaben ruft das Framework unseren Code auf.

Ein Beispiel hierfür ist [nextJs](https://nextjs.org), ein React Framework.

### Anders als Create React App

NextJS gibt uns vor, dass wir unsere Anwendung in `pages` Komponenten aufteilen.
`Pages` sind gleichzeitig unsere `Routen`. Bspw `/` oder `/about`.

Wir haben außerdem die Möglichkeit Datenquellen zu definieren `getStaticProps`, `getServersideProps` etc.
Selber aufrufen tun wir diese aber nicht.

Stattdessen regelt NextJS wann welche Logiken aufgerufen werden.

# Diagramas de base de datos (fuente Mermaid)

Cada `database-diagram-bc-0X.mmd` es la definición entidad-relación del Bounded Context
correspondiente, en sintaxis Mermaid (`erDiagram`). Los PNG de la sección 4.8.1 se generan
a partir de estos archivos, por lo que el diagrama queda versionado junto con el informe.

## Regenerar los PNG

Requisitos: Node.js y Google Chrome instalados.

```bash
npx @mermaid-js/mermaid-cli -i database-diagram-bc-05.mmd \
  -o ../database-diagram-bc-05.png -p puppeteer-config.json -b white -s 3
```

Repetir para cada Bounded Context (01 a 08). El flag `-s 3` controla la resolución.

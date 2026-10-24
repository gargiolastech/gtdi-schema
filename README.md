# gtdi-schema

JSON Schema del file di configurazione `.gtdilifetime.json` usato da **gtdi**, il tool .NET
(`Gargiolastech.DiLifetime.Tool`) che verifica lifetime e convenzioni delle registrazioni di
dependency injection in un repository C#.

Una cartella per versione del formato:

| Versione | Schema |
|---|---|
| `version: 1` (sperimentale nella serie 0.x) | [`v1/gtdilifetime.schema.json`](v1/gtdilifetime.schema.json) |

Per l'autocompletamento negli editor, all'inizio di `.gtdilifetime.json`:

```json
{
  "$schema": "https://raw.githubusercontent.com/gargiolastech/gtdi-schema/main/v1/gtdilifetime.schema.json",
  "version": 1
}
```

`gtdi init` scrive questo valore da solo; `gtdi schema` stampa lo schema incluso nel tool.
Questo repository contiene solo la copia pubblicata: la fonte dello schema e' nel repository del tool.

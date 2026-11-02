# claudeig

Repositorio preparado para trabajar con [Cursor](https://cursor.com) y Claude Code.

## Abrir en Cursor

1. Instala Cursor desde https://cursor.com/download.
2. Clona el repositorio:
   ```bash
   git clone https://github.com/mktbithome-glitch/claudeig.git
   ```
3. En Cursor: **File → Open Folder** y selecciona la carpeta `claudeig`.
4. Inicia sesión con GitHub en Cursor (**Settings → Integrations → GitHub**) si quieres usar
   los Background Agents de Cursor sobre este repositorio.

## Configuración incluida

| Archivo | Para qué sirve |
| --- | --- |
| `AGENTS.md` | Instrucciones compartidas para los agentes (Cursor y Claude Code las leen). |
| `CLAUDE.md` | Redirige a Claude Code a `AGENTS.md`. |
| `.cursor/rules/proyecto.mdc` | Regla de Cursor que se aplica siempre y referencia `AGENTS.md`. |
| `.cursor/mcp.json` | Servidores MCP del proyecto para Cursor (vacío; añade los que necesites). |

### Añadir un servidor MCP en Cursor

Edita `.cursor/mcp.json`, por ejemplo:

```json
{
  "mcpServers": {
    "mi-servidor": {
      "url": "https://ejemplo.com/mcp"
    }
  }
}
```

No pongas API keys directamente en este archivo; usa variables de entorno.

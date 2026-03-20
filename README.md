# Agente de Control de Apertura — Agencia VIO

App web que analiza documentos de despacho aduanero usando IA y determina si
la carpeta está completa para procesar la DIN.

**Corre 100% en el browser. Sin servidor. Sin instalaciones.**

---

## Cómo usar

1. Abrí la URL de GitHub Pages (ver abajo)
2. Ingresá tu API Key de Anthropic
3. Subí los documentos del despacho (PDF, JPG, PNG)
4. Hacé click en **Analizar carpeta**
5. El agente entrega el reporte en pantalla

---

## Deploy en GitHub Pages (5 minutos)

```
1. Crear repositorio nuevo en GitHub (puede ser privado)
2. Subir el archivo index.html
3. Ir a Settings → Pages
4. Source: "Deploy from a branch" → main → / (root)
5. Guardar → en 1-2 minutos aparece la URL
```

La URL queda como:
```
https://TU_USUARIO.github.io/NOMBRE_REPO/
```

Eso es todo. Compartís esa URL con Diego y ya puede usarlo.

---

## Notas técnicas

- Llama directo a `api.anthropic.com` desde el browser
- Documentos se envían como base64 (no se guardan en ningún servidor)
- La API Key se usa solo en memoria, no se almacena
- Compatible con Chrome, Firefox, Safari, Edge

---

## Próximo paso

Una vez validado el POC, este mismo agente se integra como módulo
dentro de la plataforma de gestión existente.

# Diseño

## ¿Qué hace el programa?
Este programa toma un archivo `.asm` de Hack y lo convierte a `.hack` (binario de 16 bits).
También entiende corrimientos.

## ¿Qué resuelve?
- Lee líneas normales, comentarios y etiquetas.
- Traduce instrucciones tipo A y tipo C.
- Maneja símbolos (predefinidos + variables nuevas).
- Si hay un error, dice en qué línea está.
- Si falla, borra el archivo de salida incompleto.

## ¿Cómo está organizado?
Todo está en `src/HackAssembler.py` y se divide por funciones:
- Cargar y limpiar líneas.
- Primera pasada: guardar etiquetas.
- Segunda pasada: traducir todo a binario.
- Guardar el `.hack` final.

## Flujo
1. Carga el `.asm`.
2. Guarda etiquetas con su dirección.
3. Traduce instrucciones A/C.
4. Escribe el `.hack`.
5. Si algo está mal, corta y muestra error.

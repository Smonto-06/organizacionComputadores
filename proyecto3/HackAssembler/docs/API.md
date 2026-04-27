## Tablas
- `TABLA_DEST`
- `TABLA_COMP`
- `TABLA_JUMP`
- `SIMBOLOS_PREDEFINIDOS`

## Funciones principales
- `load_commands(ruta_entrada)`
- `primera_pasada(comandos, simbolos)`
- `segunda_pasada(comandos, simbolos)`
- `ensamblar(ruta_entrada)`
- `main()`

## Funciones de apoyo
- `es_etiqueta(comando)`
- `is_a_instruction(comando)`
- `simbolo_valido(simbolo)`
- `normalizar_dest(destino)`
- `parse_c_instruction(comando)`

## Error personalizado
- `ErrorEnsamblador`

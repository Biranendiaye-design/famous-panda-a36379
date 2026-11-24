# Biiraan.SN · BSN Business

Versión 2.1 — panel para crear y seguir múltiples retos independientes.

## Funciones
- Crear tantos retos como se necesiten.
- Modalidades: reinversión del retorno, ciclo con retirada, importe manual y personalizado.
- Capital inicial configurable entre 1 € y 500 €.
- Duración de 3, 7, 10 días o personalizada (1–365 días).
- Registro diario de cantidad, cuota (1.50–10.00), resultado, retirada y notas.
- Cálculo de retorno, beneficio neto y saldo estimado.
- Calendario por reto, panel de estadísticas, resumen compartible y exportación CSV.
- Migración de retos sencillos guardados por la versión 1 cuando el navegador aún conserva esos datos.
- Sección de contacto oficial con correo `one.bsn@hotmail.com` y acceso directo a WhatsApp `+34 643 762 047`.

## Publicar en Vercel
1. Sube `index.html` y `README.md` a la raíz del repositorio GitHub conectado a Vercel.
2. Confirma el cambio en la rama `main`.
3. Vercel debería iniciar un despliegue automáticamente. Espera a que figure como `Ready` y revisa la web.

No requiere proceso de compilación: es una página estática.

## Almacenamiento y límites
Los datos se guardan en `localStorage` del navegador y dispositivo actual. No hay cuentas de usuario, base de datos remota, sincronización entre dispositivos ni autenticación. El resumen compartible usa la función nativa de compartir del dispositivo cuando está disponible; en caso contrario descarga un archivo de texto.

## Reglas de cálculo
- Ganada: retorno bruto = cantidad × cuota; beneficio neto = retorno bruto − cantidad apostada.
- Perdida: se resta la cantidad apostada.
- Anulada/devuelta: se devuelve la cantidad apostada.
- La retirada indicada se descuenta del saldo del reto.
- El siguiente importe se propone como sugerencia, no se apuesta ni se reinvierte automáticamente. El usuario debe revisar y confirmar cada registro.

La herramienta solo registra datos introducidos manualmente; no realiza apuestas ni garantiza resultados.

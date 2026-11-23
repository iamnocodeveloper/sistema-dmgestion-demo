# DM Gestión Inmobiliaria — demo del sistema de interesados

Demo navegable (una sola página, sin backend) del sistema de gestión de interesados
para **DM Gestión Inmobiliaria** (San Juan, Argentina).

## Qué muestra

- **Entrada**: botón «Entrar al sistema» y «Ver el recorrido guiado».
- **Panel del día**: interesados nuevos sin asignar, visitas de hoy, seguimientos que
  toca hacer, cierres del mes y avisos automáticos.
- **Interesados**: tabla con buscador y filtros por etapa, embudo
  (nuevo · contactado · visita agendada · en negociación · cerrado · frío) y ficha con
  datos de contacto, qué busca, propiedades mostradas, historial de la conversación y
  acciones de seguimiento (día 1 · 3 · 7).
- **Propiedades**: cartera con buscador; de cada una, interesados activos y visitas.
- **Seguimiento automático**: la secuencia que corre sola, la maqueta de los mensajes de
  WhatsApp y un interruptor para pausarla.
- **Visitas**: agenda de la semana por asesor con estado.
- **Informes**: gráficos propios (SVG/CSS) de consultas por mes, cierres por mes,
  interesados por zona y tasa de respuesta por etapa.
- **Web pública**: listado de propiedades con buscador y formulario
  «Consultar por esta propiedad» que arma el mensaje de WhatsApp al **+54 9 264 513 0508**.
- **Recorrido guiado**: tour de 7 pasos sobre la interfaz, con Atrás / Siguiente / Salir,
  contador de paso, teclado (← → Esc) y modo automático.

## Datos

Todos los datos son **de ejemplo** (nombres, barrios y montos en pesos argentinos).
No se envía ni se guarda nada: la app es estática.

## Ejecutar

```bash
docker build -t sistema-dmgestion .
docker run -p 8080:80 sistema-dmgestion
```

---

Demo de referencia hecho por **Nocodeveloper**. Los datos son de ejemplo.

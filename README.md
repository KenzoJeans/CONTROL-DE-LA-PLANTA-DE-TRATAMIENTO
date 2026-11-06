# Control de la Planta de Tratamiento – Kenzo Jeans

Dashboard para el seguimiento de la Planta de Tratamiento de Agua Residual (PTAR) de Kenzo Jeans.

## Propósito

Este repositorio se creó para dar seguimiento a todos los aspectos relacionados con la PTAR. Busca:

- Reducir el consumo de papel.
- Generar procesos más eficientes.
- Hacer el trabajo más práctico para el operario de la planta.

## ¿Qué controla el dashboard?

| Módulo | Descripción |
|---|---|
| Parámetros de vertimientos | Seguimiento de los parámetros medidos en los vertimientos de Tintorería |
| Agua tratada | Valores diarios de agua tratada |
| Mantenimiento | Registro de mantenimientos de la planta |
| Consumo de químicos (kardex) | Control del consumo de químicos en cada preparación |

## Cómo fluye la información

```
Formulario de Google  →  Hoja de cálculo (Drive de Gestión Ambiental)  →  Dashboard
```

1. El operario diligencia el formulario correspondiente.
2. Las respuestas se guardan en la hoja de cálculo **"REGISTRO DE PARÁMETROS - VERTIMIENTOS TINTORERÍA"**, en el Drive de Gestión Ambiental.
3. El dashboard lee esa hoja y muestra la información.

Hoja de cálculo (base de datos): [REGISTRO DE PARÁMETROS - VERTIMIENTOS TINTORERÍA](https://docs.google.com/spreadsheets/d/12iJMb1ujmfzng1NQ7o4iD2COwvkMvxwOrU7s92UT4Ek/edit?gid=248312250#gid=248312250)

## Formularios de reporte

Todos los formularios están creados desde el perfil de Gestión Ambiental.

| ¿Qué se reporta? | Cuándo usarlo | Enlace |
|---|---|---|
| Mantenimiento | Cada vez que se realice un mantenimiento | [Formulario](https://docs.google.com/forms/d/1nkyjquyjixniyzQY3t-Igd6hsrge1fnDb9Eiie8McKQ/edit) |
| Parámetros de vertimientos de Tintorería | Cada vez que se midan los parámetros | [Formulario](https://docs.google.com/forms/d/13DZPnW9612dWDk2xzrCBIisMhOSy5B-Cfms4w6I8maU/edit) |
| Agua tratada diaria | Una vez por día, al tomar los valores | [Formulario](https://docs.google.com/forms/d/1GKhlGf1po2-xHwpBm98M7-PUi7fS_mSbzgUERrjJokI/edit) |
| Consumo de químicos (kardex) | Cada vez que se prepare un químico | [Formulario](https://docs.google.com/forms/d/1YRx2C9OyHD2eKAjjAoV_dzM-4QHESZyJVPbf5gIOlbY/edit) |

## Reglas de diligenciamiento

- **Evite reportar en días posteriores.**
- Diligencie la información **en el momento** en que se miden los parámetros, se preparan los químicos o se realiza el mantenimiento.

Un dato reportado tarde pierde trazabilidad y puede alterar los indicadores del dashboard.

## Ejecución y despliegue

> Completar:

- **Aplicación principal:** `[nombre del archivo, p. ej. app.py]`
- **Instalar dependencias:** `pip install -r requirements.txt`
- **Ejecutar en local:** `streamlit run [archivo].py`
- **Despliegue:** Streamlit Cloud, cuenta `[completar]`, URL `[completar]`
- **Credenciales:** el dashboard necesita acceso de lectura a la hoja de cálculo. Se configuran en los *secrets* de Streamlit Cloud (nunca en el código). Detalle: `[completar dónde está documentado y quién las administra]`

## Responsables

- **Dueño del proceso:** `[Ambiental / Analista]`
- **Mantenimiento técnico del dashboard:** `[Raúl Jaimes / Analista]`
- **Cuentas (GitHub, Streamlit, Google):** `[Saúl Galvis]`

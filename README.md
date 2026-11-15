# La Bendita — Monitoreo de Cacao

App Flutter (Dart) para productores de cacao: resumen de la finca, diagnósticos, parcelas, escaneo con cámara y reportes. El diseño sigue la pantalla de inicio de referencia (La Bendita, Milagro, Guayas).

## Cómo correrla

1. Instala Flutter y agrega `C:\flutter\bin` al PATH (en esta máquina el SDK está en `C:\flutter`).
2. En la carpeta del proyecto:

```bash
flutter pub get
flutter run -d chrome
```

En Android o Windows: `flutter run`.

## Supabase

1. Crea un proyecto en [Supabase](https://supabase.com).
2. Copia `.env.example` a `.env` y completa:

```
SUPABASE_URL=https://TU-PROYECTO.supabase.co
SUPABASE_ANON_KEY=tu_anon_key
```

3. En el SQL Editor pega y ejecuta `supabase/schema.sql`.
4. Reinicia la app. Si `.env` está vacío, se muestran datos de demostración.

## Pantallas

- **Inicio**: banner, resumen, últimos diagnósticos, acciones rápidas, maduración.
- **Mis cultivos**: parcelas.
- **Escanear**: foto + resultado de IA de demostración (listo para conectar un modelo real).
- **Reportes**: indicadores y maduración.
- **Ajustes**: estado de conexión a Supabase.

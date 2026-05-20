# WaylandCraft 1.0.2

## Что нового
- Добавлен shader compatibility mode (включён по умолчанию) для лучшей совместимости с shader packs.
- Добавлен runtime-флаг `WAYLANDCRAFT_DISABLE_DMABUF_MODIFIERS` для обхода проблем DMA-BUF modifiers на части драйверов (в т.ч. NVIDIA RTX).
- Улучшена устойчивость запуска: более безопасная загрузка native-библиотеки, улучшенное логирование и обработка ошибок.
- Улучшена загрузка иконок приложений (PNG/SVG) и диагностика сбоев.
- Улучшена обработка keymap/settings (UTF-8, безопасное чтение, отказоустойчивость).
- README дополнен русским описанием и секцией с рекомендациями для NVIDIA RTX.

## Совместимость
- Minecraft: 26.1.2
- Fabric Loader: 0.19.2+
- Linux (Wayland)

## Рекомендуемые параметры для проблемных shader/GPU конфигураций
- `WAYLANDCRAFT_SHADER_COMPAT=true`
- `WAYLANDCRAFT_DISABLE_DMABUF_MODIFIERS=true`
- `__GL_THREADED_OPTIMIZATIONS=0`

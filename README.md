## Конфигурация для создания и запуска приложения обработки rtsp-потока

### Запуск

1. Выполните инструкции для следующих проектов: https://github.com/PosTour/frame_analyzer, https://github.com/PosTour/video_processor.git
2. Клонируйте репозиторий: git clone https://github.com/PosTour/video_deploy.git
3. Используйте команду в корневой папке проекта: docker compose up (docker-compose up -d)
4. При необходимости остановить работу контейнеров выполните команду: docker compose down
5. Отправьте POST-запрос со ссылкой на rtsp-поток. В терминале: Invoke-WebRequest -Uri http://localhost:8081/video/process -Method POST -Body "Ссылка" -ContentType "text/plain"
6. Для получения результатов отправьте GET-запрос по адресу http://localhost:8081/video
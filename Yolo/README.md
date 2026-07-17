# Обучение YOLO

- [`Yolo_V.ipynb`](Yolo_V.ipynb) — код подготовки датасета и обучения YOLOv8n на размеченных данных из [`../Razmetka_manual`](../Razmetka_manual).
- [`best_yolo_model_V.pt`](best_yolo_model_V.pt) — лучшие веса обученной модели (сохраняются кодом в `/content/drive/MyDrive/best_yolo_model_V.pt`).
- [`metrics/`](metrics/) — графики и логи обучения (results.csv, results.png, confusion matrix, PR/F1/P/R-кривые, labels.jpg, args.yaml).

## Полная папка с результатами обучения (Google Drive)

Полная папка со всеми выходными файлами обучения (чекпоинты по эпохам, полные логи и т.д.) выложена отдельно:

**Ссылка на папку с результатами обучения (Google Drive):** `<ВСТАВЬТЕ СЮДА ССЫЛКУ НА ПАПКУ 0000>`

## Как воспроизвести обучение

1. Скачать датасет по ссылке из [`../Razmetka_manual/README.md`](../Razmetka_manual/README.md), положить в `/content/drive/MyDrive/Labeling.zip` (Google Colab).
2. Запустить `Yolo_V.ipynb` — обучится модель, веса появятся в `/content/runs/detect/yolo_runs/bubbles_text/weights/best.pt` и будут скопированы в `/content/drive/MyDrive/best_yolo_model_V.pt`.

> Повторное обучение не обязательно — в репозитории уже лежат готовые веса (`best_yolo_model_V.pt`) и все метрики/графики обучения для ознакомления (папка `metrics/`).

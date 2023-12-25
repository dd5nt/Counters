### Новые модели YOLOv8 на DataSet-3
- **[💾 Medium 1280 200 эпох](https://drive.google.com/drive/folders/1Mp-tKrQd7t1gGNwS4wPjV968LLFWP-Z7?usp=sharing)**
- **[💾 Medium 1440 250 эпох](https://drive.google.com/drive/folders/1SBrDqFHxCpZwFpPm_k5y1ZEycn6L4AWm?usp=sharing)**
- **[💾 Small 1280 150 эпох](https://drive.google.com/drive/folders/1e3ZTxoIRzqvOHGRfhUvR_ZjQ-6hm-Fqj?usp=sharing)**

![image](https://github.com/alecseiterr/counters/assets/99917230/178aace1-1176-471f-9453-a14664c660d9)


### Итоговый дополнительный ДатаСет для Обучения YOLOv8 на дату 06.12.2023

**[📸 NewCountersDataSet 06.12.2023 ](https://drive.google.com/file/d/1rxSGicbctboRUbIGiCc01n3YcQcowzcf/view?usp=sharing)**

---

<details><summary><h4>Старые ссылки на первые части набираемого ДатаСета:</h4></summary>
<li>[DataSet-2 на 23.11.2023](https://drive.google.com/file/d/1I5DnyJalB5gC3_YY4ewWiugeCcaoFZtH/view?usp=sharing)</li>
<li>[DataSet-3 на 30.11.2023](https://drive.google.com/file/d/1upGKclAteu1MpEzLqbaGvmtTPIbS3oYm/view?usp=sharing)</li>
</p></details>

---
### Сравнение моделей YOLOv8 [Оптимальный вариант 09: cds2_s-seg_1280_100e.pt]

**[⚛️ cds2_s-seg_1280_100e.pt](https://drive.google.com/file/d/1BH3Gta5PLvJOkSwIEin8cvA9CAmlTVCC/view?usp=sharing)**

**[💾 Обученные Модели YOLOv8 на Google Drive (+Train.Logs) 💾](https://drive.google.com/drive/folders/1CqJ_nz3k6bfvA76meVZIVpBoR0s3QNeW?usp=sharing)**

![image](https://github.com/alecseiterr/counters/assets/99917230/10ce11cf-1852-4593-8d25-6b08e13e8294)

<img src="https://github.com/alecseiterr/counters/assets/99917230/1052eab6-fee4-4852-b10a-e2b4b2120b97" width=440>

<img src="https://github.com/alecseiterr/counters/assets/99917230/690396fa-b16a-4e4a-81d2-97f6b195978c" width=560>

![image](https://github.com/alecseiterr/counters/assets/99917230/9ed10a5a-acd8-4606-969c-a7edff509af8)

---

![image](https://github.com/alecseiterr/counters/assets/99917230/3a51bedd-501f-474d-bf9f-e0a31eda0432)

![image](https://github.com/alecseiterr/counters/assets/99917230/8ab5e59a-027c-4501-afee-ad5722ecccfd)


![image](https://github.com/alecseiterr/counters/assets/99917230/ef16745d-b55b-4e30-b516-85f09a8a23e6)

![image](https://github.com/alecseiterr/counters/assets/99917230/836e1f1d-b4ca-4369-afb4-8dcb0ab34d6b)

---

### Предлагаемая схема развития проекта

```mermaid
graph TD
    SwaggerUI["Swagger UI"] -->|HTTP/HTTPS| API
    CLI["CLI (url)"] -->|HTTP/HTTPS| API
    GoogleColab["Google Colab Client"] -->|HTTP/HTTPS| API
    TgBot1["Telegram Bot-1"] -->|HTTP/HTTPS| API
    TgBot2["Telegram Bot-2"] -->|HTTP/HTTPS| API
    WebClient["x Web Client.."] -->|HTTP/HTTPS| API

    API["API (FastAPI)"] -->|GPU| Docker["Docker Container"]

    Docker -->|REST| DataBase["DataBase"]
    Docker -->|REST| YOLOv8OBB["YOLOv8 OBB"]
    Docker -->|REST| YOLOv8Seg["YOLOv8 Segmentation"]
    Docker -->|REST| Keras["Keras"]
    Docker -->|REST| OCR["OCR"]
    Docker -->|REST| xBusinessLogic["x Business Logic.."]
```


### Пример результата работы YOLOv8 (первые тесты)
<details><summary><h4>TRAIN-1</h4></summary>
<img src="https://github.com/alecseiterr/counters/assets/99917230/24878214-bdba-4982-8ad6-073adeb0dfbd" alt="image" />
</p></details>

<details><summary><h4>TRAIN-2</h4></summary>
<img src="https://github.com/alecseiterr/counters/assets/99917230/5126a9c6-1d18-4ea1-ae9c-67ed1f97be14" alt="image" />
</p></details>

---

<details><summary><h2>✅ Отчет</h2></summary><p>
<h3>📆 неделя 05.09-12.09</h3>
<li>1. Изучение ТЗ и ДатаСета заказчика</li>
<li>2. Обдумывание способов разработки решения с учетом ТЗ</li>
	
<h3>📆 неделя 12.09-19.09</h3>
<li>1. Изучение популярных open source инструментов для разметки Датасетов</li>
<li>2. Продолжение изучения материалов на портале УИИ по обнаружению объектов</li>

<h3>📆 неделя 19.09-26.09</h3>
<li>1. Разметка изображений в приложении CVAT</li> 

<h3>📆 неделя 26.09-03.09</h3>
<li>1. Окончание и проверка разметки части ДатаСета [16]</li>
<li>2. Изучение форматов аннотаций CVAT, Pascal, YOLO, COCO</li>
<li>3. Первые пробы обучения YOLOv8 на малом ДатаСете</li>
</p></details>

---

<details><summary><h3>💾 ТЗ на проект "Распознавание показаний счётчиков и серийных номеров"</h3></summary><p>
<li>1. Введение Целью данного проекта является разработка системы для распознавания показаний счётчиков различных видов и серийных номеров этих счётчиков с использованием фотографий, полученных через Telegram Bot. Распознанные данные будут отправляться обратно пользователю,сверятся о отправляться в базу данных.</li><br>
	
<h4>2. Основные требования</h4>
<li>Разработать модель машинного обучения для распознавания показаний счётчиков и серийных номеров на фотографиях.
Создать Telegram Bot, интегрированный с моделью распознавания.</li>
<li>Бот должен быть способен обрабатывать фотографии счётчиков и извлекать из них числовые показания и серийные номера.
Проект должен быть способен работать с различными типами счётчиков и разными структурами серийных номеров.</li><br>

<h4>3. Описание процесса</h4>
<li>Пользователь делает фотографию счётчика с помощью смартфона и отправляет ее через Telegram Bot.</li>
<li>Telegram Bot получает фотографию и передает её на обработку модели распознавания.</li>
<li>Модель анализирует фотографию, извлекает числовые показания и серийный номер счётчика.</li>
<li>Полученные данные (показания и серийный номер) отправляются обратно пользователю через Telegram Bot.</li>
<li>Пользователь сверяет распознанные показания с реальными при необходимости корректирует.</li>
<li>Показания заносятся в базу данных с выгрузкой в файл.</li><br>

<h4>4. Требования к модели распознавания</h4>
<li>Модель должна быть обучена на достаточно большом и разнообразном датасете, чтобы достичь точности не менее 98%.</li>
<li>Модель должна поддерживать работу с различными структурами показаний счётчиков и серийных номеров.</li>
<li>Возможность переобучения модели на новых данных для улучшения качества распознавания.</li><br>

<h4>5. Требования к Telegram Bot</h4>
<li>Создать Telegram Bot, который будет интегрирован с моделью распознавания.</li>
<li>Бот должен уметь принимать фотографии от пользователей и передавать их на обработку модели.</li>
<li>После обработки моделью, бот должен отправить результаты (показания и серийный номер) пользователю.</li>
<li>Принимать скорректированные показания и вносить их в базу.</li><br>

<h4>6. Интеграция и развертывание</h4>
<li>Развернуть удаленный сервер для обработки фотографий и запуска модели распознавания.</li>
<li>Интегрировать модель и Telegram Bot на сервере для автоматической обработки запросов.</li><br>

<h4>Важное дополнение к техническому заданию</h4>
<li>1)	Предоставленного объема датасета не достаточно для достижения указанной точности в 98%. Также в датасете имеется малое количество фотографий счетчиков одного типа что не позволит обучить модель на для позиционирование серийного номера и показаний прибора. </li>
<li>2)	Нужна будет сборка сервера или аренда для работы бота.</li><br>

</p></details>

---

<details><summary><h3>Ссылки</h3></summary><p>
<li><strong><a href="">Google Colab Notebook</a></strong></li><br>
<img src="" alt="image" />
</p></details>

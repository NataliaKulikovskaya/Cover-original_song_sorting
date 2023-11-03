# Обнаружение каверов музыкальных треков
**Описание проекта:**
Разработка решения для обнаружения кавер-треков и их связывания с исходными треками важная задача, которая может значительно улучшить опыт пользователей музыкального сервиса. Цель проекта "Обнаружение каверов музыкальных треков" заключается в создании решения, способного классифицировать треки по признаку кавер-некавер, связывать каверы с оригинальными треками и находить исходный трек в цепочке каверов.
Главная цель проекта - улучшить качество рекомендаций музыкального сервиса и обогатить пользовательский опыт.

Предложенный алгоритм нужен для для определения кавер-треков, включающий анализ музыкальных метаданных и текстов песен.

**Содержание:**
Был произведен анализ исходных данных. По результатам чего мы определили, что некоторые столбцы могут быть использованы в целях машинного обучения. Кроме того, было решено что нужно дополнить данные информацией об исполнителе и дате релиза трека. С наше й точки зрения ключевой информацией является тексты песен, которые в значительной степени пропущены в исходных данных. Для создания более эффективной модели рекомендуем собрать больше данных с использованием API. Тексты песен были лемматизированы и векторизованы. Были обучены модели DecisionTreeClassifier, RandomForestClassifier, LogisticRegression,         CatBoostClassifier качество которых проверяли использованием метрик F1-score и ROC-AUC.

**Установка:**
Могут возникнуть проблемы с установкой библиотеки MusicMetaLinker. Мы использовали Google Colab. При работе с библиотекой оказалось, что подтягиваются корректные data_release, однако artist содержит в себе только 'заглушки'.

**Использование:**
Мы предлагаем это решение как пример. Для обучения более эффективной модели требуется последующий сбор данных с помощью API, на что трабуется затратить время. Мы предлагаем пользоваться musixmatch API.

**Авторы:** Анастасия Клубкова, Александра Саакян, Куликовская Наталия, Детинина Елена (менеджер проекта).

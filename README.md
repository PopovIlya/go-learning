# go-learning
Библиотеки и классы написанные в рамках курса по Go: https://www.udemy.com/course/golang-ninja/

### Memcache примеры использования
// Создаем контейнер с временем жизни по-умолчанию равным 5 минут и удалением просроченного кеша каждые 10 минут
memcache := memorycache.New(5 * time.Minute, 10 * time.Minute)

// Установить кеш с ключем "myKey" и временем жизни 5 минут
memcache.Set("myKey", "My value", 5 * time.Minute)

// Получить кеш с ключем "myKey"
i := memcache.Get("myKey")

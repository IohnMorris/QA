# Text Box Test Cases

Сайт для тестирования: https://demoqa.com/text-box

---

## Positive тесты

### Тест 1 — Успешная отправка формы Text Box

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Под формой отображаются введённые данные:

- Name: Ivan Ivanov
- Email: ivan@mail.com
- Current Address: Moscow, Tverskaya 1
- Permanent Address: Moscow, Arbat 10

---

## Тесты с пустыми полями

### Тест 2 — Отправка формы с пустым Email

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Оставить поле **Email** пустым
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Под формой отображаются данные:

- Name: Ivan Ivanov
- Current Address: Moscow, Tverskaya 1
- Permanent Address: Moscow, Arbat 10

Поле **Email** не отображается.

---

### Тест 3 — Отправка формы с пустым Current Address

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Оставить поле **Current Address** пустым
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Отображаются:

- Name: Ivan Ivanov
- Email: ivan@mail.com
- Permanent Address: Moscow, Arbat 10

Поле **Current Address** не отображается.

---

### Тест 4 — Отправка формы с пустым Permanent Address

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Оставить поле **Permanent Address** пустым
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Отображаются:

- Name: Ivan Ivanov
- Email: ivan@mail.com
- Current Address: Moscow, Tverskaya 1

---

### Тест 5 — Отправка формы с пустыми Email, Current Address и Permanent Address

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Оставить поле **Email** пустым
3. Оставить поле **Current Address** пустым
4. Оставить поле **Permanent Address** пустым
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Отображается только:

- Name: Ivan Ivanov

---

### Тест 6 — Отправка формы с пустыми полями

**Шаги**

1. Оставить поле **Full Name** пустым
2. Оставить поле **Email** пустым
3. Оставить поле **Current Address** пустым
4. Оставить поле **Permanent Address** пустым
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма отправляется.  
Под формой данные не отображаются.
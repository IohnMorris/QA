# Text Box Negative Test Cases

Сайт для тестирования: https://demoqa.com/text-box

---

## Negative тесты

### TC-001 — Неверный формат Email

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivanmail.com" в поле **Email**
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Поле **Email** подсвечивается красным и форма не отправляется.

---

### TC-002 — Email без домена

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivan@" в поле **Email**
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Поле **Email** подсвечивается красным и форма не отправляется.

---

### TC-003 — Ввод чисел в поле Full Name

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "12345" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**
Форма успешно отправляется.
Под формой отображаются введённые данные, включая значение "12345" в поле **Full Name**.

Примечание:
Поле **Full Name** принимает числовые значения.

---

### TC-005 — Ввод HTML-тегов в текстовые поля

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "<script></script>" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "<b></b>" в поле **Current Address**
4. Ввести "<style></style>" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма успешно отправляется.

Под формой отображаются введённые данные, включая HTML-теги:

- Name: `<script></script>`
- Email: `ivan@mail.com`
- Current Address: `<b></b>`
- Permanent Address: `<style></style>`

HTML-теги отображаются как текст и не выполняются.

**Примечание**

Текстовые поля принимают HTML-теги.

---

### TC-006 — Ввод одного символа в текстовые поля

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "р" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "т" в поле **Current Address**
4. Ввести "м" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма успешно отправляется.

Под формой отображаются введённые данные:

- Name: `р`
- Email: `ivan@mail.com`
- Current Address: `т`
- Permanent Address: `м`

**Примечание**

Система принимает ввод из одного символа в текстовых полях.

---

### TC-007 — Ввод двух символов в текстовые поля

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "рр" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "тт" в поле **Current Address**
4. Ввести "мм" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма успешно отправляется.

Под формой отображаются введённые данные:

- Name: `рр`
- Email: `ivan@mail.com`
- Current Address: `тт`
- Permanent Address: `мм`

**Примечание**

Система принимает ввод из двух символов в текстовых полях.

---

### TC-008 — Отправка формы с пустыми полями

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Не вводить данные в поля формы:
   - Full Name
   - Email
   - Current Address
   - Permanent Address
2. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма успешно отправляется.

Под формой не отображаются данные, так как поля были пустыми.

**Примечание**

Система допускает отправку формы с пустыми полями.

---

### TC-009 — Отправка формы с пустым Email

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Оставить поле **Email** пустым
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма отправляется.

Под формой отображаются введённые данные:

- Name: Ivan Ivanov
- Current Address: Moscow, Tverskaya 1
- Permanent Address: Moscow, Arbat 10

Поле **Email** не отображается.

---

### TC-010 — Отправка формы с пустым Current Address

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Оставить поле **Current Address** пустым
4. Ввести "Moscow, Arbat 10" в поле **Permanent Address**
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма отправляется.

Под формой отображаются:

- Name: Ivan Ivanov
- Email: ivan@mail.com
- Permanent Address: Moscow, Arbat 10

Поле **Current Address** не отображается.

---

### TC-011 — Отправка формы с пустым Permanent Address

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Ввести "ivan@mail.com" в поле **Email**
3. Ввести "Moscow, Tverskaya 1" в поле **Current Address**
4. Оставить поле **Permanent Address** пустым
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма отправляется.

Под формой отображаются:

- Name: Ivan Ivanov
- Email: ivan@mail.com
- Current Address: Moscow, Tverskaya 1

Поле **Permanent Address** не отображается.

---

### TC-012 — Отправка формы с несколькими пустыми полями

**Предусловие**

Открыта страница https://demoqa.com/text-box

**Шаги**

1. Ввести "Ivan Ivanov" в поле **Full Name**
2. Оставить поле **Email** пустым
3. Оставить поле **Current Address** пустым
4. Оставить поле **Permanent Address** пустым
5. Нажать кнопку **Submit**

**Ожидаемый результат**

Форма отправляется.

Под формой отображается только:

- Name: Ivan Ivanov
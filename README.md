# Практична робота 6

### Команда інсталяції
``
pip install selenium
``


## Завдання 1 - Відкрити контекстне меню

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/context_menu)
### [Посилання на навчальний матеріал](https://www.selenium.dev/documentation/webdriver/actions_api/mouse/)


## Завдання 2 - Автоматизувати checkbox

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/checkboxes)
### [Посилання на навчальний матеріал](https://www.selenium.dev/documentation/webdriver/actions_api/mouse/)

## Завдання 3 - Нескінченний скрол

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/infinite_scroll)
### [Посилання на навчальний матеріал](https://www.selenium.dev/documentation/webdriver/actions_api/wheel/)

## Завдання 4 - Ввід даних

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/inputs)
### [Посилання на навчальний матеріал](https://pythonexamples.org/python-selenium-enter-value-in-input-text/)

## Завдання 5 - Вибір елементів з випадаючого списку

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/dropdown)
### [Посилання на навчальний матеріал](https://А-це-самі-давайте)



---
## Завдання варто документувати на кожному етапі через print() або logging.info() у консоль
## У звіт обов'язково вставити код або посилання на репозиторій, знімки екранів під час виконання програми та консоль

---

### Для написання коду використовуйте контекстний мененджер:
```python
with closing(webdriver.Chrome()) as driver:
    driver.get("https://opensource-demo.orangehrmlive.com/web/index.php/auth/login")

    driver.implicitly_wait(3)
    element = driver.find_element(by=By.NAME, value="username")
```
### Він автоматично закриває з'єднання з сайтом

### Деякі приклади використання пошуку за атрибутами чи типом:
```python
driver.find_element(by=By.NAME, value="username")
driver.find_element(by=By.ID, value="firstname")
driver.find_element(by=By.CSS_SELECTOR, value='button[type="submit"]')
driver.find_element(by=By.PARTIAL_LINK_TEXT, value="My Info")

```

# Корисні матеріали:
### [Відеоурок](https://www.youtube.com/watch?v=NB8OceGZGjA&t=3s)
### [Невеличкий туторіал по базових командах](https://www.geeksforgeeks.org/selenium-python-tutorial/)
# Практична робота 6

### Команда інсталяції
``
pip install selenium
``

## Завдання 1 - Знайти усі елементи на сторінці. Вивести у консоль назву та посилання 

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/)
### [Посилання на навчальний матеріал](https://www.geeksforgeeks.org/locating-multiple-elements-in-selenium-python/)

## Приклад
1. A/B Testing - https://the-internet.herokuapp.com/abtest
2. Add/Remove Elements - https://the-internet.herokuapp.com/add_remove_elements/
3. ...

## Завдання 2 - Автоматизувати дію (Action) Drag-and-Drop (Взяти і перемістити)

### [Посилання на тестовий сайт](https://the-internet.herokuapp.com/drag_and_drop)
### [Посилання на навчальний матеріал](https://www.geeksforgeeks.org/drag_and_drop-action-chains-in-selenium-python/)

### На сайті необхідно знайти два елементи та поміняти їх місцями


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
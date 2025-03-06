# Практична робота 8

### Команда інсталяції
``
pip install selenium
``


## Завдання - Симуляція дій користувача на вебсайті

### [Посилання на тестовий сайт](https://www.saucedemo.com/)
### [Посилання на навчальний матеріал](https://а-це-самі-давайте)

1. Вхід на сайт
2. Переглянути кожен товар
3. Додати два товари до корзини
   * Товари на ваш вибір

Після завершення попередніх етапів:
4. Перейти до корзини
5. Видалити один з товарів
6. Оформити та підтвердити замовлення іншого
7. Перейти на головну сторінку
8. Вийти з сайту
   * Необхідно зробити вихід користувача з сайту через кнопку Logout

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
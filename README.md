# HW4: DML, DDL та Складні SQL-запити (Olist E-commerce)

**Назва датасету:** Olist Brazilian E-commerce Public Dataset

**Офіційне джерело:** [Kaggle: olistbr/brazilian-ecommerce](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

**Спосіб отримання файлів:**
Файли завантажуються програмно та автоматично за допомогою Python-бібліотеки `kagglehub` безпосередньо у середовищі Google Colab під час виконання першого блоку коду. Дані спочатку імпортуються у проміжні `raw`-таблиці за допомогою `pandas`, після чого переносяться у `typed`-схему з відповідними обмеженнями (constraints) засобами SQL-запиту `INSERT ... SELECT`.

**Sample-розмір (кількість рядків):**
Датасет містить інформацію про приблизно 100 тис. замовлень. За результатами автоматичного smoke-тесту, фінальні типізовані таблиці мають такий обсяг:
* `olist_order_items`: 112 650 рядків
* `olist_customers`: 99 441 рядок
* `olist_orders`: 99 441 рядок
* `olist_order_reviews`: 99 224 рядки
* `olist_products`: 32 951 рядок
* `olist_sellers`: 3 095 рядків

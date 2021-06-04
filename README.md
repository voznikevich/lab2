# Звіт до лабораторної роботи 2
### Тема: _Представлення телекомунікаційних мереж у термінах теорії графів._
### Мета роботи: _Навчитись представляти телекомунікаційні мережі за допомогою матриць суміжності, інцедентності та списку ребер, і оволодіти основними поняттями теорії графів._
---
## Хід роботи
1. Записати (придумати) матрицю суміжності орієнтованого графа `G={7,12}`. Ввести її у лабораторний макет та побудувати візуальне представлення графа.
   
   ![матриця суміжності](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-06%2000-04-28.png)
   ![граф](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-06%2000-04-50.png)
   
    1. Чи є у побудованому графі ізольовані вершини або незв’язні компоненти? *Tак* - назвіть їх; *Hі* - які ребра потрібно видалити щоб вони утворились? 
    
    **Відповідь: Немає. Якщо видалити ребра (1, 3), (2, 6) та (5, 2), утворяться незв’язні компоненти. Якщо видалити ребра (0, 1) та (0, 2), утвориться ізольована вершина.**
    
    3. Чи є у графі вершини типу _глухий кут_? *Так* - то змінивши напрямок ребер чи можна це усунути; *Hі* - вкажіть цикл обходу всіх вершин;
    
    **Відповідь: Так, вершина 0. Це можна усунути, якщо змінити напрямок ребра (0, 1) або (0, 2).**
    
    4. Чи існує в графі цикл обходу вершин (_цикл Гамільтона_)? *Так* - вкажіть послідовність вершин, що входять до даного циклу; *Hі* - що потрібно змінити в графі щоб даний цикл існував;
    **Відповідь: Не існує. Потрібно змінити напрямок деяких ребер.**
    5. Чи існує в графі цикл обходу ребер (_цикл Єйлера_); *Так* - вкажіть послідовність ребер, що входять до даного циклу; *Hі* - що потрібно змінити в графі щоб даний цикл існував;
    **Відповідь: Не існує. Для існування циклу Ейлера необхідно, щоби не більше ніж дві вершини мали непарний степінь.**
    6. Побудувати доповнення (обернений) графа `G`.
    ![vffg](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-18%2023-33-20.png)
    ![fg](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-18%2023-33-02.png)
1. За допомогою лабораторного макету побудувати випадковий неорієнтований граф `G={7,15}` та записати його матрицю суміжності.
 
 ![граф](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-06%2000-52-23.png)
 
 ![матриця суміжності](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-06%2000-52-42.png)
	
1. За допомогою лабораторного макету побудувати випадковий орієнтований граф `G={5,10}` та записати його матрицю відповідностей (інцедентності).
![alt](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-18%2023-42-47.png)
![alt](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-18%2023-42-25.png)
	1. Як з матриці відповідностей можна визначити ступінь кожної вершини?
   **Відповідь: по кількості одиниць у рядку матриці, який позначає певну вершину.**
1. Задано граф `G` та `M`.
    ```python
       G={(5,1), (6,1), (2,3), (3,4), (2,6), (3,6), (5,6), (1,7), (2,7), (3,7), (4,7), (6,7)}
       M={(2,1), (5,1), (1,2), (4,2), (5,2), (6,2), (2,4), (5,4), (6,4), (1,5), (2,5), (4,5), (6,5), (2,6), (4,6), (5,6)}
    ```
    Визначте для кожного з графів:
    1. Записати їх матриці суміжності та побудувати графічне представлення.
    
    **Граф G**
    ![матриця суміжності G](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-17%2013-46-14.png)
    ![граф G](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-17%2013-46-31.png)
    **Граф M**
    ![граф M](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-17%2013-23-56.png)
    ![матриця суміжності M](https://github.com/Maksym-Horchyn/lab-2/blob/main/Screenshot%20from%202021-04-17%2013-23-42.png)
    2. Графи орієнтовані чи неорієнтовані? 
    **Відповідь:** 
    **Граф G - орієнтований.**
    **Граф М - неорієнтованим.**
    3. Яка кількість вершин `V` та ребер `E`?
    **Відповідь:** 
    **Граф G: V = 7, E = 12.** 
    **Граф М: V = 6, E = 8.**
    4. Яка з вершин має найбільшу ступінь? Скільки?
    **Відповідь:**
    **Граф G: вершини 1 та 2 мають ступінь 3.** 
    **Граф М: вершини 1 та 4 мають ступінь 4.**
    5. Визначте ексцентриситети вершин для графа `G` та `M`.
    **Відповідь:**
    **Граф G: 2** 
    **Граф М: 2**
    6. Який радіус кожного з графів?
    **Відповідь:**
    **Граф G: 1** 
    **Граф М: не є зв'язним**
    7. Який діаметр кожного з графів?
    **Відповідь:**
    **Граф G: 2** 
    **Граф М: не є зв'язним**
    8. Чи містять графи петлі (елементарні цикли)? Вкажіть послідовність ребер.
    **Відповідь: не містять.**
    9. Чи містять графи ізольовані вершини?

    **Відповідь: Граф М містить ізольовану вершину 2.**

    10. При транспонування `G` та `M` чи змінюється графічне представлення графа? Як?
    ### Висновок: 

    **Відповідь:**

    **Граф G: ** 
    **Під час виконання даної роботи за допомогою Graph Online було побудовано декілька графів та розглянуто основні поняття теорії графів: орієнтований та неорієнтований граф, матрииці суміжності та інцидентності, цикли обходу. ексцентрисет, діаметр, радіус графа, ступінь вершини.**

    **Граф М: **

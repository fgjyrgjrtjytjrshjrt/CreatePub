# PR3
## Algorithms Sort Massive C++ 

![alt](https://www.google.com/imgres?imgurl=https%3A%2F%2Fi.stack.imgur.com%2FUinhu.jpg&tbnid=NxmdOMgZUKUznM&vet=12ahUKEwiFhvfq2cyBAxWBs4sKHY2ICtUQMygAegQIARBM..i&imgrefurl=https%3A%2F%2Fru.stackoverflow.com%2Fquestions%2F1196615%2F%25D0%259D%25D0%25B5-%25D1%2580%25D0%25B0%25D0%25B1%25D0%25BE%25D1%2582%25D0%25B0%25D0%25B5%25D1%2582-%25D0%25BA%25D0%25BE%25D0%25B4-%25D0%25BF%25D1%2580%25D0%25BE%25D1%2581%25D1%2582%25D0%25B5%25D0%25B9%25D1%2588%25D0%25B0%25D1%258F-%25D0%25B7%25D0%25B0%25D0%25B4%25D0%25B0%25D1%2587%25D0%25B0&docid=DtrNvFCRxTtXzM&w=478&h=305&q=rjl%20c%2B%2B&ved=2ahUKEwiFhvfq2cyBAxWBs4sKHY2ICtUQMygAegQIARBM "shih-tzu")

'''cpp
#include <iostream>

main( )
setlocale(LC_ALL, "russian"); 
    const int size = 5;
    int mas[size];
    int tmp;
    // Введення даних у масив користувачем
    for (int i = 0; i < size; i++){
        cout << "Введіть " << i << " елемент масиву ";
        cin >> mas[i];
    }
    // Виведення масиву на екран
    for (int i = 0; i < size; i++){
        cout << "Елемент з індексом " << i << " має значення " << mas[i] << endl;
    }
    // Сортування масиву бульбашкою
    int x = 0;
    for (int i = size - 1; i >= x; i--)
    {
        for (int j = size - 1; j >= x; j--)    {
            if (mas[j] < mas[j-1])    {
                tmp = mas[j];
                mas[j] = mas[j-1];
                mas[j-1] = tmp;
                cout << "елемент " << j << " помінявся з елементом " << j - 1 << " << " << endl; // наводка
                                    }

                                            }
        x++;
    }
    // виведення відсортованого масиву
    cout << "Виведення відсортованого масиву" << endl;
    for (int i = 0; i < size; i++){
        cout << "Елемент з індексом " << i << " має значення " << mas[i] << endl;
    }
    system("pause");
    return 0;
}
'''

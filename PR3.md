# PR3
## Algorithms Sort Massive C++ 



'''cpp
#include <iostream.h>
#include <conio.h>
main( )
{ const int n = 5;
  int x[n], i, k;  int а;       /* а — рабочая переменная для перестановки местами двух элементов */
//----------- ввод исходного массива
  for (і = 0; і < n; i++)
   сіn >> *(x+i);
//----------- вывод на экран исходного массива
  cout << "\n massiv х[n] \n";
  for (i = 0; i < n; i++) 
  cout << *(x+i) << " "; 
//------------- сортировка no возрастанию
  for (k = 1; k < n; k++)       // цикл шагов сортировки
    for (і = 0; і < n-k; і++)    /* цикл сравненья элементов и их перестановки */
    if (*(x+i) > *(x+i+1))   
    { а = *(x+i);
     *(x+i) = *(x+i+1);
     *(x+i+1) = a; }
  cout << "\n Result sortirovki massiva " << endl;
  for (i=0; і < n; i++) 
  cout << *(x+i) << " ";
  getch();  
}
'''

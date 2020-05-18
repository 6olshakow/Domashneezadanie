# Domashneezadanie
Дз для ШАГА
Урок n 7(Многомерные массивы)
1)
#include<stdlib.h>
#include <iostream>

using namespace std;

int main()
{
setlocale(LC_ALL, "Russian");
const int row=3;
const int col=4;
int A[row][col];
srand(time(NULL));
int summ=0;
for(int i=0;i<row;i++)
{
for(int j=0;j<col;j++)
{
A[i][j]=rand()%10;
cout<<A[i][j]<<"\t";
if (A[i][j]==0)
summ++;
}
cout<<"\n\n";
}
cout<<"Количесво нулей в массиве равно "<<summ<<"\n";
}

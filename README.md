# Programa 4

Linguagem Utilizada: C++.

Programa com menu que pode converter temperatura de Celsius para Fahrenheit e vice versa, calcular o volume de uma lata e determinar a quantidade de litros de combustível utilizado por um veículo em uma viagem.

Programa desenvolvido no DEV C++ IDE. 

Código:

#include "iostream"
#include "cstdlib"
#include "math.h"
#include "string.h"
#include "conio.h"
using namespace std;

int main(){
    setlocale (LC_ALL, "portuguese");

    float F,C;
    double altura,raio,volume;
    float distancia,tempo,velocidade,litros_usados;

    string clas;

	char tecla = '0';

	while(tecla != 27)

	{
                system("cls");
                cout << "\n1 - Converter a temperatura de Celsius para Fahrenheit\
                         \n2 - Converter a temperatura de Fahrenheit para Celsius\
                         \n3 - Calcular o volume da lata de óleo\
                         \n4 - Calcular a quantidade de litros de combustível usados em uma viagem\
                         \nESC - Sair";
                tecla = getch();


	if (tecla == '1')
	{

    system("cls");
	cout << "Digite a temperatura em graus celsius: "; cin >> C;
	cout << "\n";
    F = (9 * C + 160) / 5;
    cout << "A temperatura em Fahrenheit é: " << F << endl;
    cout << "A temperatura em Celsius é: " << C << endl;
	cout << "\n";
	system("pause");
    }

    else if (tecla == '2')
    {

    system("cls");
	cout << "Digite a temperatura em graus Fahrenheit: "; cin >> F;
	cout << "\n";
    C = (F - 32) * (0.55555);
    cout << "A temperatura em Celsius é: " << C << endl;
    cout << "A temperatura em Fahrenheit é: " << F << endl;
	cout << "\n";
	system("pause");
    }

    else if (tecla == '3'){
    system("cls");
    cout << "Digite o raio da lata de óleo: "; cin >> raio;
    cout << "\n";
    cout << "Digite a altura da lata de óleo: "; cin >> altura;
    cout << "\n";

    volume = 3.14159 * raio * raio * altura;

    cout << "O volume da lata é: " << volume << endl;
    system("pause");
    }

    else if (tecla == '4') {
    system("cls");
    cout << "Digite o tempo: "; cin >> tempo;
    cout << "\n";
    cout << "Digite a velocidade: "; cin >> velocidade;
    cout << "\n";
    system("cls");

    distancia = tempo * velocidade;

    litros_usados = distancia/12;
    
    cout << "A velocidade media foi: " << velocidade << endl;
    cout << "O tempo gasto foi: " << tempo << endl;
    cout << "A distância percorrida foi: " << distancia << endl;
    cout << "Os litros usados foram: " << litros_usados << endl;
    system("pause");
    }

    }

    system("pause");

return 0; }

# Estudos-

#include <iostream>
using namespace std;

// apresentar uma função
void texto();
void soma(int n1, int n2);
int soma2(int n1, int n2);
void tr(string tra[2]);

int main(){

string transp[2]=("carro","moto","barco");

int res;
soma(15,5);
res=soma2(175,25);
cout << res << "\n";
tr(transp);
return 0;
}


void texto (){

cout << "\nOla mundo\n";

}
//nao retorna nada, sem valor de retorno
// fica parado atévoid tr(string tra[4]) ser chamado
void soma(int n1, int n2){
   cout << "\nA soma dos valores: " << n1+n2 << "\n";

}

int soma2(int n1, int n2){
return n1+n2;
//retorno
}
void tr(string tra[2]){

for (int i=0; i<3; i++){
    cout << tra[i] << "\n";
    }
}


#Cadeia de caracteres, string
frase = 'luisinho' #carrega os caracteres dentro da memoria com numeros sequenciais 
# tecnica de fatiamento 
frase[9:13] #vai de 9 a 13 porem o 13 num conta
frase[9:21:2] #terceiro seria a possibilidade de skip de caracteres 
frase[:5] #começa do caractere 0 
frase[15:] #15 até o final 
frase[9::3] #va icomeçar no 9 , vai até o final, de 3 em 3 

#Analise 

len(frase) #comprimento *
frase.count('o') #contar quantas vezes o 'o' aparece
frase.count('o',0,13) #fatiamento 
frase.find('deo') # Encontra na string/ caso nao exista retorna valor -1
'curso' in frase # Dentro da frase existe a string na frase 

#Transformação

frase.replace('Python','Android') #Troca
frase.upper() #Em maiusculas
frase.lower() #Em minusculas
frase.capitalize() #Joga tudo pra minusculo e a primeira letra se mantem maiusculo 
frase.title() #Analisa quantas palavras tem pela posição dos espaços colocando o primeiro caracter em maiusculos
frase.strip() #remove os espaços exedentes no começo e no final 
frase.rstrip() #r - trata pelo lado direito, excluindo apenas os caracteres a extrema direita 
frase.lstrip() #l- esquerda...............

#Divisão 
frase.split() #como fazer um split, divisão considerando os espaços 
#Junção
'-'.join(frase) #une a string através do q esta entre as aspas 


#ler o nome completo/ nome com todas as letras maiusculas/ nome com todas minusculas/Quantas letras tem/ Quantas letras tem o primeiro nome 
"""
Nome = input('Qual o seu nome?  ')
print(Nome.upper())
print(Nome.lower())
ContadorLetras = len(Nome.replace(" ",""))
SplitName = Nome.split()
Contador1Nome = len(SplitName[0])
print(Contador1Nome)
print(ContadorLetras)

#Faça um programa que le um numero de 0 a 9999 e mostre na tela cada um dos digitos separados

Num = input('escreva um numero:  ')
Num1 = Num[0]
Num2 = Num[1]
Num3 = Num[2]
Num4 = Num[3]
print('Primeira letra: {}'.format(Num1))
print('Segunda letra: {}'.format(Num2))
print('terceira letra: {}'.format(Num3))
print('Quarta letra: {}'.format(Num3))
"""
#crie um programa que leia o nome de uma cidade e diga se ela começa com a palavra 'santo'
#com silva em qualquer lugar // in 
#Faça um programa quye leia uma frase pelo teclado/ quantas vezes aparece a letra a/em que posição ela aparece na primeira vez/ que posição ela aparece na ultima vez

frase = str(input('Digite uma frase:  '))
print('O a apareceu {}'.format(frase.count('a')))
print('A primeira está em {}'.format(frase.find('a')))
print('A segunda está em {}'.format(frase.rfind('a')))

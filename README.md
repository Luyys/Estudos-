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

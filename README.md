#include <iostream>

struct nodo{
	int informacion;
	struct nodo *siguiente;
	
	int main(){
	struct nodo *tope;
	struct nodo *nuevo;
	struct nodo *auxiliar;
	tope=NULL;
	int dato;
	int cantidad;
	int i=0;
	cout<<"Ingrese la cantidad de nodos que desee"<<endl;
	cin>>cantidad;
	while(i<cantidad){

		nuevo=(struct nodo *)malloc(sizeof(struct nodo));
	nuevo->siguiente=tope;
	cout<<"Ingrese Dato"<<endl;
	cin>>dato;
	nuevo->informacion=dato;
	tope=nuevo;
		i++;
	}
while(nuevo!=NULL){
	cout<<nuevo->informacion<<",";
	nuevo=nuevo->siguiente;
}
	return 0;

}

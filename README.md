#include <iostream>
using namespace std;
int main(){

    int horas,minutos,segundos,horasf,minutosf,segundosf,horasn,horasr,minutosr,segundosr;
    

    cout<<"Horas Iniciales:";
        cin>>horas;
    cout<<"Minutos Iniciales:";
        cin>>minutos;
    cout<<"Segundos Iniciales:";
        cin>>segundos;
    cout<<"Horas Finales:";
        cin>>horasf;
    cout<<"Minutos Finales:";
        cin>>minutosf;
    cout<<"Segundos Finales:";
        cin>>segundos;
if (horas <=23 && minutos<=59)
{
	if (segundos <=59 && segundosf<=59)
   {
		if (horasf <=23 && minutosf<=59)
		{
 			  horasr=horasf-horas;
 			  minutosr=minutosf-minutos;
  		  	  segundosr=segundosf-segundos;
 
 			  if (segundosr<0)
 				  {
  				  	segundosr+=60;
  				  	
  				 	minutosr-=1;
 				  }
 			  if (minutosr<0)
 				  {
  				  	minutosr+=60;
  				  	
  				 	horasr-=1;
 				  }
 			  if(horasr<0)
 				  { 
 				    horasr+=24;
				  }
  
   	       cout<<"Tu total de horas trabajadas Son:"<<horasr<<":"<<minutosr<<":"<<segundosr;
        }
   }
}
else 
{
cout<<"Las Horas o minutos no deben ser mayores de 6o";
}
    return 0;
}

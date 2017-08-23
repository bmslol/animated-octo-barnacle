# animated-octo-barnacle
#include <iostream>
using namespace std;
int main()
{

    float horas, minutos, segundos, horas2, minutos2, segundos2, total, total2, total3;

    cout<<"Ingresa la informacion en formato de 24hrs(INICIO)"<<endl<<endl;

    do{

        cout<<"Ingresa las horas de inicio"<<endl;
        cin>>horas;

    }while (horas < 0 || horas > 24);

    do{

        cout<<"Ingresa los minutos de inicio"<<endl;
        cin>>minutos;

    }while (minutos < 0 || minutos > 60);

       do{

        cout<<"Ingresa los segundos de inicio"<<endl;
        cin>>segundos;

    }while (segundos < 0 || segundos > 60);

    cout<<endl;

    cout<<"Total: "<<horas<<":"<<minutos<<":"<<segundos<<endl<<endl;


    cout<<"Ingresa la informacion en formato de 24hrs(FINALES)"<<endl<<endl;



   do{

        cout<<"Ingresa las horas finales"<<endl;
        cin>>horas2;

        if(horas2 < horas)
        {
            cout<<"ERROR"<<endl;
        }


    }while (horas2 < 0 || horas2 > 24 || horas2 < horas );

    do{

        cout<<"Ingresa los minutos finales"<<endl;
        cin>>minutos2;

    }while (minutos2 < 0 || minutos2 > 60);

       do{

        cout<<"Ingresa los segundos finales"<<endl;
        cin>>segundos2;

    }while (segundos2 < 0 || segundos2 > 60);

    cout<<endl;

    cout<<"Total: "<<horas2<<":"<<minutos2<<":"<<segundos2<<endl<<endl;

    total=horas-horas2;
    total2=minutos-minutos2;
    total3=segundos-segundos2;

if ( horas < horas2)
{
    total=total*=-1;

if (minutos < minutos2)

    total2=total2*=-1;

if (segundos < segundos2)

    total3=total3*=-1;


cout<<endl;

cout<<"Las horas trabajadas son: "<<total<<":"<<total2<<":"<<total3<<endl;
}
    return 0;
}

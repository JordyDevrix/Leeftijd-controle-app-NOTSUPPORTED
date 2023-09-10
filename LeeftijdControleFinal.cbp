#include <stdio.h>
#include <stdlib.h>
#include <time.h>
#include <unistd.h>

int main()
{
    system("cls");

    time_t t = time(NULL);
    struct tm tm = *localtime(&t);

    int jaar = tm.tm_year + 1900;
    int maand = tm.tm_mon + 1;
    int dag = tm.tm_mday;

    int hour = tm.tm_hour;
    int minute = tm.tm_min;
    int sec = tm.tm_sec;

    int jaarmin = tm.tm_year + 1882;
    int maandmin = tm.tm_mon + 1;
    int dagmin = tm.tm_mday;

    int gebjaar;
    int gebmaand;
    int gebdag;


while(1){
    printf("Securo Leeftijdscontrole");
    printf(" | Datum vandaag: %d-%d-%d | V1.0.3 | BETA | %d:%d:%d\n",dag,maand,jaar,hour,minute,sec);             //VERSIE /V_._._/
    printf("//////////////////////////////////////////////////////////////////\n");
    printf("GEBOORTE DATUM MOET EERDER ZIJN DAN %d-%d-%d.\n",dagmin,maandmin,jaarmin);
    printf("\n");
    printf("Vul het jaar in dat op het ID bewijs staat.");
    printf("\n");
fflush(stdout);
    scanf("%d", &gebjaar);

    if(gebjaar >= jaar){
        printf("voer een realistisch getal in");
        printf("\n      Opnieuw proberen?.");
    }
    if(jaar - gebjaar >= 100){
        printf("Let op, de datum die nu ingediend is, geeft aan dat de persoon 100+ is. Check goed of dit klopt.\n");
    }

    if(gebjaar < jaarmin){
        printf("Leeftijd akoord");
    }
    if(gebjaar == jaarmin){
        //jaar is goed
        printf("gelieve de maand invullen \n");
        scanf("%d", &gebmaand);

        if(gebmaand < maandmin){
            printf("Leeftijd akoord");
        }
        if(gebmaand == maandmin){
            //maand is goed
            printf("gelieve de dag invullen \n");
            scanf("%d", &gebdag);

            if(gebdag == dagmin){
                //dag is goed
                printf("Leeftijd akoord");
            }

            else if(gebdag > dagmin){
                //dag is fout
                printf("Leeftijd niet akoord!\n");
                int wachtdag;
                wachtdag = gebdag - dagmin;
                if(wachtdag == 1){
                printf("U moet helaas nog %d dag wachten tot u oud genoeg bent.\n", wachtdag);
            }
                else if(wachtdag > 1){
                printf("U moet helaas nog %d dagen wachten tot u oud genoeg bent.\n", wachtdag);
            }
            }


        }
        else if(gebmaand > maandmin){
            //maand is fout
            printf("Leeftijd niet akoord!\n");
            int wachtmaand;
            wachtmaand = gebmaand - maandmin;
            if(wachtmaand == 1){
            printf("Helaas, u moet nog %d maand wachten tot u oud genoeg bent.\n", wachtmaand);
            }
            else if(wachtmaand > 1){
            printf("Helaas, u moet nog %d maanden wachten tot u oud genoeg bent.\n", wachtmaand);
            }
        }

    }
    else if(gebjaar > jaarmin && gebjaar < jaar){
        //jaar is fout
        printf("Leeftijd niet akoord! \n");
        int wachtjaar;
        wachtjaar = gebjaar - jaarmin;
        printf("U moet nog minimaal %d jaar wachten tot u oud genoeg bent. \n", wachtjaar);
    }

    printf("\n      Druk op een willekeurige toets om door te gaan.\n");
        getch();
        return main();

        sleep(1);
        //editlog
        //V1.0.0 - basis versie
        //V1.0.1 - toevoeging 100+ check
        //V1.0.2 - bug fixes
        //V1.0.3 - bug fixes (100+ check bugs).

        //KNOWN BUGS
}
}

#include <stdio.h>
#include <stdlib.h>
#include <math.h>

int main(){
int tahminedilensayi,tahminin,tahminsayisi,score=100;
srand(time(NULL));
tahminedilensayi=(rand()%100)+1;
printf("Sayi tahmin oyununa hosgeldin\n");
printf("Sayimi tahmin et amcik\n");


while(tahminin!=-1){
printf("1-100 arasinda gir");
scanf("%d",&tahminin);
if(tahminin==-1) break;
if(tahminin<1 || tahminin>100){
printf("\n1-100 arasinda gir amina koymiyim\n");
continue;
}
tahminsayisi++;
if(tahminin==tahminedilensayi){
printf("Helal aminagoyim %d. seferde bildin",tahminsayisi);
break;}
else{
if(tahminin>tahminedilensayi){
printf("Daha kucuk bir sayi gir mal\n");
}
else{
printf("Daha buyuk sayi gir salak\n");
}
score-=10;
}
}
printf("\n Puanin 100 uzerinden %d\n",score);



return 0;
}

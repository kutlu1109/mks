#include<stdio.h>
#include<math.h>
int sayi1,sayi2,islem,sonuc;
int main(){
	
	printf("Birinci sayiyi giriniz: ");
	scanf("%d",&sayi1);
	printf("Ikinci sayiyi giriniz: ");
	scanf("%d",&sayi2);
	printf("+ toplama\n");
	printf("- cikarma\n");
	printf("* carpma\n");
	printf("/ bolme\n");
	printf("^ us alma\n");
	printf("! kok alma\n");
	printf("islem seciniz: ");
	scanf("%d",&islem);
	switch(islem)
	{
		case ' + ' : sonuc=sayi1+sayi2;
		printf("Sonucunuz: %d",sonuc); break;
		case ' - ' : sonuc=sayi1-sayi2;
		printf("Sonucunuz: %d",sonuc); break;
		case '*' : sonuc=sayi1*sayi2;
		printf("Sonucunuz: %d",sonuc); break;
		case '/' : sonuc=sayi1/sayi2; 
		printf("Sonucunuz: %d",sonuc); break;
		case '^' : sonuc=pow(sayi1,sayi2);
		printf("Sonucunuz: %d",sonuc); break;
		case '!' : sonuc=sqrt(sayi1); 
		printf("Sonucunuz: %d",sonuc); break;
		default: printf("Hatali islem kodu");
	}
}

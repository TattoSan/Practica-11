#include <stdio.h>
#include <stdlib.h>
#include <string.h>
//#include <direct.h>
#include <ctype.h>
int main()
{
	FILE *doc;
	char nombrearchivo[20];
	char descripcion_archivo[100]="";
	int numcaracter;
	printf("Nombre del archivo:");
	gets(nombrearchivo);
	fflush(stdin);
	strcat(nombrearchivo,".txt");
	doc = fopen(nombrearchivo,"r");
	if(doc == NULL)
	{
		printf("El archivo no existe '%s'.\n",162,nombrearchivo);
		return 0;
	}

	fflush(stdin);
	numcaracter=sizeof(descripcion_archivo);
	fread(&descripcion_archivo,numcaracter,1,doc);
	descripcion_archivo[0]=toupper(descripcion_archivo[0]);
	printf("\n%s\n",descripcion_archivo);
	fclose(doc);
	system("pause");
	return 0;
}

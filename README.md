#include <stdio.h>
#include <stdlib.h>
int main ()
{
	float idade, anos, dep, sal, salb, salir;
	printf ("informe o valor do salario bruto:\n");
	scanf ("%f", &salb);
	printf ("informe a quantidade de anos trabalhados:\n");
	scanf("%f", &anos);
	printf ("informe a quantidade de dependentes:\n");
	scanf ("%f", &dep);
	printf ("informe a idade do funcionario:\n");
	scanf ("%f", &idade);
	if (idade>50) {
		sal=((salb+(sal*anos*0.02)+(sal*dep*0.05)+(sal*0.03)*1.03));
		printf ("o salario liquido e:\n", sal);
	}
	else (idade<50) {
		sal=(salb+(sal*anos*0.02)+(sal*dep*0.05)+(sal*0.03));
		printf ("o salario liquido e:\n", sal);
	}
	if (sal>1000) {
		salir=(sal-(sal*0.03));
		printf ("o salario final e:\n", salir);
	}
	system ("pause");
}

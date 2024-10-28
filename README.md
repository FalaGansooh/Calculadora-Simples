Realizando uma calculadora simples

#include <stdio.h>

int main(void) {

  float N1, N2, Resultado;
  int Operador;

  printf ("Digite o primeiro número: ");
  scanf("%f", &N1);

  printf ("Digite o segundo número:");
  scanf("%f",&N2);

  printf ("Digite o operador:\n");
  printf ("1 - Adição\n");
  printf ("2 - Subtração\n");
  printf ("3 - Multiplicação\n");
  printf ("4 - Divisão\n");
  
  scanf("%d", &Operador);

  switch (Operador){

    case 1:
    Resultado = N1+ N2;
    printf("Resultado: %.2f\n", Resultado);
    break;

    case 2:
    Resultado = N1 - N2;
    printf("Resultado: %.2f\n", Resultado);
    break;

    case 3:
    Resultado = N1 * N2;
    printf("Resultado: %.2f\n", Resultado);
    break; 

    case 4:
    if (N2 != 0){
    Resultado = N1 / N2;
    printf("Resultado: %.2f\n", Resultado);
    }

    else {
      printf("Erro: Divisão por zero\n");
    }
    break;
    default:
    printf("Operador inválido\n");
    break;
  }

  return 0;
}
    
  

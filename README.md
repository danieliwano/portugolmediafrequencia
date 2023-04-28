# portugolmediafrequencia
programa
{
	
	funcao inicio()
	{
		real nota1, nota2, nota3, media
	inteiro frequencia,aulas_presentes, falta
	
	escreva ("qual a primeira nota \n")
	leia (nota1)
	escreva ("qual a segunda nota \n")
	leia (nota2)
	escreva ("qual a terceira nota \n")
	leia (nota3)

	escreva ("a frequência do aluno de 100 aulas:")
	leia (aulas_presentes)

	se(nota1 > 10.0 ou nota2 > 10.0 ou nota3 > 10.0){
   escreva("Alguma das notas digitadas são maiores que 10.0. Tente novamente.")
   inicio()
   retorne}
   	
	media = (nota1 + nota2 + nota3) / 3
	falta = aulas_presentes - 100

	//frequencia = (aulas_presentes /100) *100

	se (media >= 5 e aulas_presentes >= 75) {
	escreva("Aluno aprovado com média ", media, " e frequência de ", aulas_presentes)
	}
	
	senao se (media < 5) {
	escreva ("Aluno reprovado com média abaixo de 5")
	}
	
	senao se (aulas_presentes < 75){
	escreva ("Aluno reprovado com frequência abaixo de 75%")
	}

	
	escreva("\n Média final: \n", media)
	escreva("\n frequência: \n", aulas_presentes, "%" )
	escreva("números de faltas", falta)
	
	
	 
	
	//senao
      //escreva("Aluno reprovado por frequência.")
	

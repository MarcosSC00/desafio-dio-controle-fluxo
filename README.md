# desafio-dio-controle-fluxo

Esse projeto consiste em um sistema de que realiza uma contagem a partir de valores inseridos pelo usuário.

Esses valores são passados como parâmetro do método `contar(parametroUm, parametroDois)` da classe `Contador` o qual lança uma exceção a partir de uma condição determinada. Caso a exceção não seja lançada é relaizada uma interação com base no valor da variável `contagem`.

```java
public static void contar(parametroUm, parametroDois) throws ParametrosInvalidosException {

  if('condição'){
    throw new ParametrosInvalidosException();
  }
  int contagem = parametroDois - parametroUm;
  // exibição das mensagens por meio de laços de repetição

}
```

## A classe ParametrosInvalidosException

Como podemos ver o método `contar()` lança a exceção `ParametrosInvalidosException` que é responsável por lidar com os erros ou imprevistos ocorrido no contexto do nosso programa.

Nessa exceção, que é estendida da classe `Exception`, passamos para o contrutor o metodo `super()` com uma mensagem descrevendo a exceção em seu parâmetro. 

```java
public class ParametrosInvalidosException extends Exception{

	private static final long serialVersionUID = 1L;
	
	public ParametrosInvalidosException() {
		super("O segundo parâmetro deve ser maior que o primeiro");
	}
	
}
```

>[!IMPORTANT]
>O método `super()` é uma chamada ao construtor da classe pai `Exception`

>[!TIP]
>Esse projeto foi realizado com base no conteúdo apresentado no curso `Controle de Fluxo` ofertado pela [DIO](https://www.dio.me).

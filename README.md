# learning-java

- Repositório para anotações da Aceleração em Java da Trybe

### Variáveis e seus tipos <h3>

![image](https://user-images.githubusercontent.com/24492328/180890216-e9523dd1-e6b4-4f50-9eb1-2199648946e1.png)

- Cada tipo primitivo tem um valor default de inicialização e ocupa um espaço específico em memória. Os tipos primitivos também possuem limite de armazenamento.

![Captura de tela de 2022-07-25 20-16-26](https://user-images.githubusercontent.com/24492328/180890355-e2fefe25-fb3f-4989-9ae8-8b8a6e799d6b.png)

- float e boudle

Na inicialização de variáveis do tipo float, é necessário adicionar a letra f no final do número. O motivo é que a precisão entre float e double são diferentes. Se não inserirmos a letra f, o Java entenderá que você está tentando atribuir um valor do tipo double a uma variável do tipo float. A variável do tipo double aceita os mesmos valores do byte, short, int, long e float, além de números de ponto flutuante dentro do range double.

```
public class TiposPrimitivos {
    public static void main(String[] args) {
        float numA = -101.23f;
        float numB = 2.356f;
        System.out.println(numA + numB); // -98.874
    }
}
```
- bool
```
public class TiposPrimitivos {

    public static void main(String[] args) {
        boolean isBoolean = true; // outros exemplos: isGreaterThan, isFlexible, isStarted
        boolean ehNumero = false; // outros exemplos: ehMaiorDeIdade, ehCedo, ehValido
    }
}
```
- String builder
```
public class ObjetosString {

    public static void main(String[] args) {
        StringBuilder stringBuilder = new StringBuilder();
        String eu = "Eu";
        String ja = " já";
        String sei = " sei";
        String usar = " usar";
        String strings = " Strings";
        String em = " em";
        String java = " Java";

        String frase = stringBuilder.append(eu)
                .append(ja)
                .append(sei)
                .append(usar)
                .append(strings)
                .append(em)
                .append(java)
                .toString();
        System.out.println(frase); // Eu já sei usar Strings em Java
    }
}
```



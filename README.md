# Teste de PSI Modelo

## Informação do aluno

    Nome: Catarina Feliciano Cachoeira

Teste termina às 09:40 (Turno 1) / 13:25 (Turno 2).

Escreve as respostas dentro dos blocos correspondentes.
Substitui as reticências pelo que é pedido em cada pergunta.
Não desformates o documento.

### 1. Indica o que é impresso pelo seguinte código. Justifica a tua resposta

    char c = '\u00AE';
    Console.WriteLine($@"\n{c}\n");

P1 - Resposta

    Como a string tem @, os caracteres de escape \n não são considerados como quebras de linha. Portanto, sendo assim o resultado será a própria string.

### 2. Considera o seguinte código

    double d = 0.3513;
    float f = 12.645;

    Console.WriteLine($"{d} + {f} = {d + f}");

### Indica a correção necessária para que o código não apresente erros. Explica porque foi necessário fazer essa correção

P2 - Resposta

    float d = 0.3513;
    float f = 12.645;

    Console.WriteLine($"{d} + {f} = {d + f}");
    
    Justificação: O erro ocorre porque as variáveis d e f tem tipos diferentes, e o operador + não pode ser usado a operandos de tipos diferentes.
    Portanto, é necessário trocar uma das variáveis para o tipo da outra antes de realizar a operação.

### 3. Escreve um programa que solicite uma string ao utilizador, e seguidamente a mostre no ecrã de forma invertida

P3 - Resposta

    
    static void Main(string() args)
    {
        Console.Write("Adicione uma string: ");
        string inputString = Console.ReadLine();

        char[] charArray = inputString.ToCharArray();
        Array.Reverse(charArray);
        string reverseString = new string(charArray);

        Console.WriteLine("A string invertida é: "{0}", reversedString);
    }
    

### 4. Quais são os comandos Git para configurares, de uma forma global, o teu **nome** e **email** para realização de *commits*? E se essa configuração for apenas para um repositório?

P4 - Resposta

    git config --global user.name "Meu Nome"
    git config --global user.email "seu-email@pessoa.com"
    Se eu quiser configurar o meu nome e email apenas para um repositório específico, posso usar os mesmos comandos sem a flag --global dentro do diretório do repositório.
    


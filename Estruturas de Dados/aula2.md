# Estruturas de Dados
    Anotações da aula
    Data: 25/08/2025

---
## Vetores

- Vetores são definidos pelo tipo de dados que eles devem armazenar e a quantidade de posições.
    - Exemplo: Vetor de 8 posições para armazenar números reais;
    - Exemplo: Vetor de 40 posições para armazenar caracteres.

- **Vetor sempre começa na posição 0.**
- Vetores têm tamanho fixo, ou seja, uma vez definidos, não podem ser redimensionados.

- Estrutura de dados unidimensionais;
- Índice único que controla as posições;
```
<Tipo><Nome>[<tamanho>]
```
- Acessando a uma posição:
    - Não é possível acessar um vetor todo;
```
<nome>[<indice>]
```
- Lista de inicialização: preenche um vetor todo de uma só vez
<tipo> <nome> [<tam.>] = {<v1>, <v2>, <v3>, ..., <vn>};

# Um algoritmo que apresente 5 números inteiros e realize a media aritmética entre eles

```cpp
    #include <iostream>

    int main()
    {
        int v[5];
        float media;
        
        v[0]=50;
        v[1]=40;
        v[2]=30;
        v[3]=20;
        v[4]=10;
        
        media = (v[0]+v[1]+v[2]+v[3]+v[4])/5.0;
        
        std::cout<<"A média aritmética dos número é: "<<media<<std::endl;

        return 0;
    }
```

```cpp
    #include <iostream>

    int main()
    {
        float v[5] = {10, 20, 30, 40, 50};
        int i;
        float s = 0;
        
        for(i=0; i<5; i++){
            s+=v[i];
        }
        
        std::cout<<"A média aritmética dos número é: "<<s/5<<std::endl;

        return 0;
    }
```

```cpp
    #include <iostream>

    int main()
    {
        float v[5];
        int i;
        
        for(i=0; i<5; i++){
            std::cout<<"Insira um número: ";
            std::cin>>v[i];
        }
        
        std::cout<<"Dados inseridos:\n";
        for(i=0; i<5; i++){
            std::cout<<v[i]<<"\n";
        }

        return 0;
    }
```

```cpp
    #include <iostream>

    int main()
    {
        char nomes[5][50];
        int i;
        
        std::cout<<"Digite os nomes:\n";
        
        for(i=0; i<5; i++){
            std::cout<<"Nome "<<i+1<<": ";
            std::cin>>nomes[i];
        }
        
        std::cout<<"\nNomes digitados:\n";
        for(i=0; i<5; i++){
            std::cout<<nomes[i]<<"\n";
        }

        return 0;
    }
```
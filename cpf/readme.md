# Lista  do que precisa ser feito
- [x] Iniciar projeto
- [ ] Criar a pagina html 
- [ ] Estilizar com CSS  
- [ ] Criar a logica para validar o CPF 


# Logica para verificar digito verificador

> 0 7 4 6 3 0 5 1 9 - 2 7     <== Verificar se eh valido  

```
  0 7 4 6 3 0 5 1 9 
X 1 2 3 4 5 6 7 8 9 
  ------------------ 
  0 1 1 2 1 0 3 8 8  | 
    4 2 4 5   5   1  | soma = 189    
                           
                              189 / 11 = 17,18  

                              Como o resultado nao foi inteiro pega apenas a primeira parte

                              17 x 11 = 187

                              189 - 187 = ** 2 ** (Primeiro digito verificador)

  0 7 4 6 3 0 5 1 9 2
X 0 1 2 3 4 5 6 7 8 9
  --------------------
  0 7 8 1 1 0 3 7 7 1 | 
        8 2   0   2 8 | soma = 172

                              172 / 11 = 15,63 

                              Como o resultado nao foi inteiro pega apenas a primeira parte

                              15 x 11 = 165

                              172 - 165 = ** 7 ** (Segundo digito verificador)

```
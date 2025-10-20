# Atividade-10---2
Calculadora de IMC/Nutrição


- Descrição: API que calcula IMC e classifica o resultado; pode sugerir faixa (OMS).

- Endpoints Sugeridos:

  - Método GET /imc?peso=70&altura=1.75

  - Método GET /imc/classificacao?peso=70&altura=1.75

- Exceções personalizadas:

  - InvalidHeightException (altura <= 0 ou fora do intervalo plausível)

  - InvalidWeightException (peso <= 0 ou fora do intervalo plausível)

  - DivisionByZeroLikeException (altura zero)

- Regras/validações (Validator):

  - Altura em metros entre 0.5 e 2.5, peso entre 2 e 400 kg

- Controller + Service:

  - Controller chama serviço que calcula IMC e retorna DTO com valor e classificação

Obs.: DTO => Data Transfer Object (Objeto de Transferência de Dados). É um padrão de design de software usado para transferir dados entre diferentes camadas de uma aplicação ou entre sistemas distribuídos.

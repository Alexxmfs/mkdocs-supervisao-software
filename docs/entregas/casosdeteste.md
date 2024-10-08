# Casos de Testes

## Teste 1: Navegação Autônoma Simples
- **Objetivo:** Verificar se o carro é capaz de navegar por um percurso simples sem obstáculos.
- **Entrada:** Percurso reto com marcações no chão.
- **Esperado:** O carro deve seguir o percurso sem necessidade de intervenção humana.
- **Resultado Esperado:** Sucesso na navegação sem colisões.

## Teste 2: Desvio de Obstáculo
- **Objetivo:** Testar a capacidade do carro de identificar e desviar de obstáculos.
- **Entrada:** Colocar um objeto no percurso.
- **Esperado:** O carro deve identificar o objeto e desviar, retomando o trajeto original.
- **Resultado Esperado:** O carro deve evitar a colisão.

## Teste 3: Reconhecimento de Pistas
- **Objetivo:** Verificar se o carro pode reconhecer e seguir diferentes tipos de pistas (linhas de cores diferentes).
- **Entrada:** Pistas com linhas de diferentes cores.
- **Esperado:** O carro deve seguir a linha correta indicada.
- **Resultado Esperado:** O carro segue a linha correta sem perder a trajetória.

## Teste 4: Tempo de Resposta na Nuvem
- **Objetivo:** Avaliar o tempo de resposta do sistema ao processar imagens na nuvem.
- **Entrada:** Trajetos com diferentes tempos de resposta.
- **Esperado:** O tempo de resposta deve ser inferior a 500ms.
- **Resultado Esperado:** O carro não deve sofrer atrasos perceptíveis na execução.

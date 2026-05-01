# Relatório de Desenvolvimento: Auditoria Financeira e Simulação Espacial

## 1. Algoritmo de Auditoria de Dados (Financeiro)

### Descrição do Projeto
Este algoritmo foi desenvolvido para atuar como uma camada de segurança em sistemas de processamento de vendas[cite: 1]. Ele automatiza a verificação de transações para identificar anomalias financeiras e ajustar parâmetros de risco em tempo real[cite: 1].

### Funcionalidades Técnicas
* **Monitoramento de Média Global**: O sistema calcula a média de um conjunto de vendas e a compara com um limite de segurança pré-definido[cite: 1].
* **Estado de Quarentena**: Caso a média das transações ultrapasse o limite de R$ 100.000,00, o sistema aciona um alerta de "Quarentena"[cite: 1].
* **Detecção de Outliers**: O script verifica se alguma venda individual é superior a cinco vezes a média do grupo, sinalizando a necessidade de revisão manual[cite: 1].
* **Ajuste de Limite Dinâmico**: Após a análise, o limite de segurança é atualizado automaticamente para o valor da média atual, permitindo que o sistema se adapte ao volume de vendas do período[cite: 1].

### Aprendizados Aplicados
* Manipulação de variáveis globais para persistência de dados[cite: 1].
* Implementação de lógica condicional composta para validação de integridade de dados[cite: 1].

---

## 2. Simulador de Navegação e Evacuação Espacial

### Descrição do Projeto
Este projeto consiste em um motor de simulação que utiliza o conceito de Máquina de Estados para gerenciar o percurso de um agente em um cenário de evacuação crítica. O objetivo é navegar por diferentes locais e gerenciar recursos limitados para alcançar a saída.

### Funcionalidades Técnicas
* **Mapeamento de Cenários**: O ambiente é estruturado através de listas que correlacionam locais (Sala, Corredor, Portão) com seus respectivos estados lógicos.
* **Gerenciamento de Inventário**: O sistema monitora a coleta de itens (chave) necessários para desbloquear caminhos e avançar na simulação.
* **Lógica de Backtracking**: Caso o agente encontre um obstáculo trancado (portão) sem o item necessário, o algoritmo força o retorno para posições anteriores para buscar o item em falta.
* **Consumo de Recursos**: Cada iteração no laço de movimentação consome unidades de energia, estabelecendo uma condição de falha caso o recurso se esgote antes da conclusão do objetivo.

### Aprendizados Aplicados
* Controle de fluxo complexo utilizando laços `while` com múltiplas condições de parada.
* Manipulação dinâmica de listas para representar o inventário do agente.

---

## Tecnologias Comuns Utilizadas
* Linguagem: Python 3.x[cite: 1]
* Ferramentas de Desenvolvimento: Google Colab e Python CLI[cite: 1]

[Voltar ao início](https://github.com/seu-usuario/seu-repositorio)

---
title: Cartão de experimento
summary: Saída padrão do modo "diagnóstico de gargalo". Uma variável, uma métrica, um prazo e regra de parada obrigatória.
uso: Sempre que o diagnóstico apontar um elo quebrado. Um cartão por vez.
---

# Cartão de experimento

> **Regra:** um cartão = **uma** variável. Se você mudar duas coisas, não saberá qual funcionou.
> A **regra de parada é obrigatória** — sem ela, o experimento vira hábito.

---

```
ELO DO DIAGNÓSTICO:   [1 alcance | 2 qualidade | 3 conversão | 4 capacidade | 5 retenção]

HIPÓTESE:
  Se eu [MUDANÇA ÚNICA E CONCRETA],
  então [MÉTRICA] muda de [VALOR ATUAL] para [VALOR ALVO],
  porque [MOTIVO BASEADO EM EVIDÊNCIA].

UMA VARIÁVEL:
  A única coisa que muda:
  O que permanece igual (para não contaminar):

MEDIÇÃO:
  O que é contado:            [métrica exata]
  Quem conta:                 [nome]
  Onde é registrado:          [sistema/planilha]
  Frequência da leitura:      [diária | semanal]

PRAZO:
  Início:                     [data]
  Fim:                        [data]
  Ponto de checagem:          [data intermediária]

REGRA DE PARADA (obrigatória):
  Encerro e não insisto se:   [critério objetivo]

CUSTO:
  Tempo:                      [horas]
  Dinheiro:                   [valor ou R$ 0]

EVIDÊNCIA NECESSÁRIA (degrada sem isto):
  ☐ número do cliente   ☐ prova autorizada   ☐ dado próprio verificável

RESULTADO (preencher ao final):
  Data:                       [data]
  Valor medido:               [valor]
  Leitura:                    ☐ funcionou  ☐ não funcionou  ☐ inconclusivo
  Decisão:                    ☐ manter  ☐ reverter  ☐ escalar  ☐ novo teste
```

---

## Como escrever uma boa hipótese

| Ruim | Bom |
|---|---|
| "vou melhorar o e-mail" | "se eu trocar o assunto para o número que ele citou, a taxa de resposta sobe de 4% para 8%" |
| "vou prospectar mais" | "se eu enviar 30 toques/semana no segmento X, terei 6 respostas em 3 semanas" |
| "vou melhorar o preço" | "se eu apresentar as 3 camadas com a recomendada marcada, a taxa de fechamento sobe de 15% para 25%" |

## Erros que invalidam o experimento
- mudar duas variáveis ao mesmo tempo
- não definir o valor **atual** antes de começar (sem linha de base, não há leitura)
- prazo tão longo que o contexto muda no meio
- não ter regra de parada — o teste vira rotina permanente sem conclusão
- ler o resultado com viés de confirmação (só ver o que confirma a hipótese)

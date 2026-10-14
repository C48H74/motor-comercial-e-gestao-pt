---
title: Arquitetura do motor comercial
summary: Como o motor é montado — os três modos, a árvore de decisão por situação, o diagnóstico antes de concluir e os contratos de saída. Inclui a decisão de escopo do projeto.
---

# 11. Arquitetura do motor comercial

> Esta é a "planta" que amarra todos os outros arquivos. Leia quando precisar entender **como as
> peças se conectam**, ou quando o pedido não se encaixar claramente em um único módulo.

## 11.1 A arquitetura em 4 etapas

```
1. ESCOLHER O MODO             2. CARREGAR SÓ O NECESSÁRIO
   revisão · diagnóstico ·        árvore de decisão por situação
   construção completa            aponta para 1 módulo
              ↓                              ↓
3. DIAGNOSTICAR ANTES          4. CONTRATO DE SAÍDA
   de concluir                     veredito · diagnóstico · plano
   alcance → lead → conversão
   → capacidade → retenção
   "pare no primeiro elo quebrado"
```

## 11.2 Árvore de decisão por situação

| Situação declarada | Módulo que carrega |
|---|---|
| Oferta ou preço vago | oferta e precificação (`references/02-*`) |
| Outbound frio, sem resposta | outbound + sequência de 5 toques (`references/04-*`) |
| Primeira call | descoberta SPIN + guia de call (`references/03-*`) |
| Negócio grande | scorecard MEDDPICC (`references/03-*`) |
| Negócio travado | JOLT + biblioteca de objeções (`references/03-*`, `references/04-*`) |
| Um único contato | multithreading + mapa do comitê (`references/03-*`) |
| "Preciso de mais clientes" | diagnóstico dos 5 elos (`references/05-*`) |
| Oferta ou movimento novo | mapa de 12 passos (`references/05-*`) |

## 11.3 Diagnóstico antes de concluir

**Ordem obrigatória, sem pular:**

```
Alcance → Qualidade do lead → Conversão → Capacidade → Retenção
```

**"Pare no primeiro elo quebrado."** Otimizar conversão quando o problema é alcance é desperdício de
esforço e de credibilidade. Cada elo limita os seguintes — não existe atalho.

## 11.4 Contratos de saída

| Modo | Saída obrigatória | Onde está o template |
|---|---|---|
| **Revisão rápida** | veredito em 1 frase + artefato corrigido | — (a saída é o próprio artefato) |
| **Diagnóstico de gargalo** | diagnóstico por elo + **1** cartão de experimento | `templates/cartao-de-experimento.md` |
| **Construção completa** | plano + templates + donos e prazos em 30 dias | `templates/plano-30-60-90.md` |

## 11.5 Ativos do motor (inventário de referência)

O motor original foi desenhado com este inventário. Use como meta de completude:

| Ativo | Quantidade de referência | Situação nesta skill |
|---|---|---|
| Referências | 17 | **12** arquivos de referência (consolidados) |
| Templates | 9 | **13** templates |
| Roteiros operacionais | 3 | **3** roteiros completos (validação, venda consultiva, negociação) |
| Biblioteca de objeções | 15 objeções | estrutura + 7 objeções catalogadas (`references/04-*`) |
| Checklists | 2 | checklist de anti-padrões + checklists por módulo |
| Exemplos anotados | 2 | 1 exemplo calibrado (§11.6) |

> **Lacuna declarada:** a biblioteca completa de 15 objeções e os 2 exemplos anotados do desenho
> original **não foram reproduzidos** porque as fontes disponíveis não os continham. Está registrado
> como próximo passo.

## 11.6 Exemplo calibrado — revisão rápida

**Pedido:** *"meu cliente disse que R$ 12.000/ano é caro. O que eu respondo?"*

**Modo:** revisão rápida. **Módulos:** objeções + valor (MEDDPICC M) + JOLT T.

> **Veredito:** isso não é objeção de preço — é **valor não quantificado**. Você nunca colocou um
> número no lado esquerdo da balança.
>
> **O que fazer, nesta ordem:**
> 1. Não defenda o preço. Número absoluto sem comparação sempre parece caro.
> 2. Volte à dor e quantifique: *"quantas horas por semana sua equipe gasta emitindo nota
>    manualmente?"* → horas × custo/hora × 52 = **o número dele**.
> 3. Traga prova de cliente do mesmo porte — **com autorização**.
> 4. Se ainda travar, é **risco**, não preço: ofereça saída, não desconto (JOLT, T).
> 5. Revise as camadas: talvez você ofereceu a completa para quem precisa da essencial.
>
> **Evidência necessária:** número da dor dele + um caso autorizado. **Sem os dois, não responda.**
>
> **Armadilha:** "consigo um desconto" — destrói a âncora e não resolve a causa.

## 11.7 Decisão de escopo da skill

Esta skill cobre **duas frentes** com um roteador. A decisão foi deliberada:

- **Frente comercial:** proxied pelo pedido sobre vender, precificar, prospectar, negociar.
- **Frente de entrega:** acionada quando o assunto é prazo, custo, escopo, risco, status.
- **O roteador:** o `SKILL.md` decide pela situação declarada, não pelo histórico.

**Por que unir as duas:** o motor comercial promete e a gestão de entrega cumpre. Separadas, a
primeira vende o que a segunda não sustenta — que é exatamente o que o efeito bola de neve e a falta
de handoff produzem (ver `references/06-entrega-projetos.md` e `templates/plano-30-60-90.md`).

**Alternativa considerada e descartada:** duas skills separadas, com leitura cruzada. Descartada
porque o ponto de falha mais comum está justamente **na fronteira** entre vender e entregar.

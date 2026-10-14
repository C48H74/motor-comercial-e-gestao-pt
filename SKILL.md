---
name: motor-comercial-e-gestao-pt
description: Motor comercial e gestão de entrega para negócios B2B de ciclo complexo. Use para revisar ou corrigir oferta, preço ou e-mail; diagnosticar por que a receita travou (alcance, qualidade do lead, conversão, capacidade, retenção); conduzir descoberta e qualificação (SPIN, MEDDPICC, Challenger, JOLT); montar proposta, garantia e plano 30/60/90; e para planejar, controlar e reportar projetos (PMBOK 7, valor agregado, riscos, ISO 21502/31000). Não use para análise de código-fonte nem para parecer jurídico formal.
whenToUse: Quando o pedido envolver vender melhor (oferta, preço, objeção, pipeline, descoberta, proposta) ou entregar melhor (escopo, prazo, custo, risco, status de projeto). Não acione para arquitetura de software ou consultoria jurídica/tributária.
---

# Motor Comercial e Gestão de Entrega

Skill de duas frentes que se conectam: **vender** (motor comercial) e **entregar** (gestão de projeto).
A frente comercial promete; a frente de entrega cumpre. Usar uma sem a outra quebra o negócio.

## Regras que valem acima de todas as outras

1. **Evidência acima de adjetivo.** Nenhuma afirmação sem origem: pessoa, número, data ou documento.
2. **Pare no primeiro elo quebrado.** Não otimize conversão quando o problema é alcance.
3. **Nunca invente número, depoimento ou caso.** O que falta vira `[a preencher]`.
4. **Sem o arquivo de perfil, a saída é genérica.** Se `templates/perfil-negocio.md` não estiver
   preenchido, avise o usuário e pergunte o mínimo necessário antes de produzir.

## Como operar

> **Antes de tudo:** se a oferta **nunca foi vendida** (ou é nova), o passo é **validar com dinheiro
> real** — não estruturar. Ver `templates/roteiro-validacao-de-ideia.md`. Estruturar oferta, preço e
> outbound antes de alguém pagar é o erro mais caro do começo, e o mais comum porque "parece
> profissional".

### Passo 1 — Escolha o menor modo que responde

| Modo | Gatilho | Entrega obrigatória |
|---|---|---|
| **Revisão rápida** | um e-mail, um preço, uma objeção | veredito em 1 frase + artefato corrigido |
| **Diagnóstico de gargalo** | "preciso de mais clientes", "não converte" | 5 verificações com veredito + 1 cartão de experimento |
| **Construção completa** | oferta nova, produto novo, movimento novo | mapa de 12 passos + templates + donos em 30 dias |

Não faça os três de uma vez. Pedido rápido recebe resposta rápida.

### Passo 2 — Carregue só o módulo necessário

| Situação declarada | Arquivo a ler |
|---|---|
| Oferta vaga, preço vago, valor mal comunicado | `references/02-oferta-e-precificacao.md` |
| Outbound frio, ninguém responde | `references/04-outbound-e-objecoes.md` |
| Primeira call, descoberta, perguntas a fazer | `references/03-metodologias-de-venda.md` |
| Negócio grande, qualificação, previsão de fechamento | `references/03-metodologias-de-venda.md` |
| Cliente convencido que não decide ("vou pensar") | `references/03-metodologias-de-venda.md` (JOLT) |
| Um único contato na conta | `references/03-metodologias-de-venda.md` (comitê) |
| Mapa completo, 12 passos, portões de funil | `references/05-motor-comercial-12-passos.md` |
| Projeto estourou prazo ou custo | `references/07-custos-e-previsao.md` |
| Escopo que não para de crescer | `references/06-entrega-projetos.md` |
| Não sei por que a receita travou | `references/05-motor-comercial-12-passos.md` |
| Risco, ameaça, oportunidade, reservas | `references/08-risco.md` |
| Reuniões, papéis, kickoff, rotina do gestor | `references/09-pessoas-e-rituais.md` |
| Governança, conformidade, ISO, benchmarks | `references/10-normas-e-benchmarks.md` |
| Validação de ideia, venda consultiva, negociação (escola brasileira) | `references/12-validacao-e-negociacao-br.md` |
| Entender como as peças se conectam, ou pedido que não encaixa em um módulo | `references/11-arquitetura-do-motor.md` |
| Dúvida sobre evidência, honestidade, o que prometer | `references/01-evidencia-e-perfil.md` |
| Cliente que comprou e não usa, churn, renovação | `references/05-motor-comercial-12-passos.md` (elo 5, retenção) |
| Precisa preencher o contexto do negócio | `templates/perfil-negocio.md` |

Leia **um** arquivo. Só leia um segundo se o primeiro apontar explicitamente para ele.

### Passo 3 — Escolha o template de saída

| O que você vai produzir | Use o template |
|---|---|
| Contexto do negócio (fazer **primeiro**) | `templates/perfil-negocio.md` |
| **Validar ideia com dinheiro real** (antes de tudo) | `templates/roteiro-validacao-de-ideia.md` |
| **Conduzir reunião de venda consultiva** | `templates/roteiro-venda-consultiva.md` |
| **Preparar e conduzir negociação** | `templates/roteiro-negociacao-integrativa.md` |
| Oferta, camadas de preço e garantia | `templates/proposta-e-garantia.md` |
| Resultado do diagnóstico (modo 2) | `templates/cartao-de-experimento.md` |
| Plano de entrega, adoção e retenção | `templates/plano-30-60-90.md` |
| Autorizar formalmente um projeto | `templates/termo-de-abertura.md` |
| Reportar status ao patrocinador | `templates/relatorio-de-status.md` |
| Definir papéis e responsabilidades | `templates/matriz-raci.md` |
| Registrar e acompanhar riscos | `templates/registro-de-riscos.md` |
| Conduzir a reunião de abertura | `templates/roteiro-de-kickoff.md` |
| Revisar a entrega antes de enviar | `templates/checklist-anti-padroes.md` |

### Passo 4 — Verifique antes de entregar

Percorra a **escada de evidência** (`references/01-evidencia-e-perfil.md`) e diga em que degrau
a entrega está. Não chame de funcional o que está apenas escrito.

### Passo 5 — Feche com o contrato de saída

- **Específico:** "poste na terça às 9h" — não "poste nas redes".
- **Opinativo:** "mate esta funcionalidade" — não "considere despriorizar".
- **Com fonte:** todo número externo com origem. Sem origem → "Estimativa" ou "Não encontrado".
- **Breve:** limite de palavras. Brevidade força clareza.
- **Estruturado:** tabelas, checklists e matrizes — nunca parede de texto.
- **Com veredito:** termine com **avançar / corrigir / descartar**.

## Mapa da skill

```
motor-comercial-e-gestao/
├── SKILL.md                              ← este arquivo (roteador)
├── references/
│   ├── 01-evidencia-e-perfil.md          escada de evidência, o que prometer, como preencher o perfil
│   ├── 02-oferta-e-precificacao.md       6 modelos, 3 camadas, garantia com exposição
│   ├── 03-metodologias-de-venda.md       SPIN, MEDDPICC, comitê, JOLT, Challenger
│   ├── 04-outbound-e-objecoes.md         sequência de 5 toques, objeções, fraseado honesto
│   ├── 05-motor-comercial-12-passos.md   os 12 passos, portões, diagnóstico dos 5 elos
│   ├── 06-entrega-projetos.md            PMBOK 7, escopo, documentos, status, kickoff, decisão
│   ├── 07-custos-e-previsao.md           EVM, PERT, previsão, controles, qualidade
│   ├── 08-risco.md                       matriz, estratégias, reservas, pitfalls de medição
│   ├── 09-pessoas-e-rituais.md           4 reuniões, RACI, rotina, maturidade, delegação
│   ├── 10-normas-e-benchmarks.md         ISO 21502, ISO 31000, PMI Pulse (parte não verificada)
│   ├── 11-arquitetura-do-motor.md        os 3 modos, árvore de decisão, contratos de saída
│   └── 12-validacao-e-negociacao-br.md   Meisler e Alfredo Soares; testar antes de estruturar
└── templates/
    ├── perfil-negocio.md                 contexto do negócio (pré-requisito de tudo)
    ├── roteiro-validacao-de-ideia.md     testar demanda com dinheiro real
    ├── roteiro-venda-consultiva.md       diagnóstico e recusa disciplinada
    ├── roteiro-negociacao-integrativa.md previsibilidade, escolha fechada, troca de concessões
    ├── cartao-de-experimento.md          saída padrão do modo diagnóstico
    ├── plano-30-60-90.md                 entrega, adoção e retenção
    ├── termo-de-abertura.md              TAP
    ├── relatorio-de-status.md            os 5 blocos
    ├── matriz-raci.md                    papéis
    ├── registro-de-riscos.md             exposição por risco
    ├── proposta-e-garantia.md            oferta, camadas, garantia
    ├── roteiro-de-kickoff.md             pauta com tempos e registro de decisões
    └── checklist-anti-padroes.md         11 categorias de revisão
```

## Limites conhecidos desta skill

- **Números das metodologias de venda** (ex.: "40% dos melhores são Challenger", "17% de aumento no
  estudo SPIN") vêm dos próprios autores, **sem verificação independente**. Trate como afirmação de
  origem, nunca como fato medido.
- **ISO 21502 e ISO 31000** foram sintetizadas de exposições de terceiros, não do texto oficial.
  Antes de citar parágrafo de norma, consulte o texto.
- **A referência 12** (Meisler, Alfredo Soares) é **opinião de praticante**, extraída de um
  compilado de vídeos cujas atribuições e trechos **não foram verificados por mim**. Trate como
  referência de mercado; se for citar nominalmente para cliente, confirme a fonte original.
- **Fora do escopo:** jurídico, tributário, contábil formal, análise de código-fonte.
- **Números do PMI Pulse** (ref. 10 §10.3): só o crescimento de 57% no híbrido e a afirmação de desempenho equivalente foram confirmados na página oficial. Percentuais por ano, a amostra de 477 empresas e os 8 facilitadores **não** foram confirmados. Não cite sem conferir o relatório.
- **Números de SPIN:** o "17% de aumento" não é afirmação de Rackham e não deve ser usado (ref. 03 §3.1).
- **Lacuna aberta:** finanças de pequeno negócio (margem, ponto de equilíbrio, fluxo de caixa,
  imposto) e aquisição por canal além de outbound.

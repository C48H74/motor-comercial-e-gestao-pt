# motor-comercial-e-gestao

Skill de agente (formato `SKILL.md` com referências e templates) para **motor comercial** (oferta, preço, venda, negociação) e **gestão de entrega de projetos** (PMBOK 7, valor agregado, riscos, ISO 21502/31000), em português.

## Estrutura

```
SKILL.md          roteador: regras, modos de operação, mapa de módulos
references/      12 módulos de conteúdo (01 a 12)
templates/       13 modelos de saída (roteiros, planos, registros, checklists)
scripts/         validadores de estrutura e de frontmatter
```

## Validação

```bash
node scripts/validar_skill.mjs .        # estrutura, frontmatter, referências cruzadas
npm install yaml && node scripts/validar_yaml.mjs .   # frontmatter com o parser YAML
```

Ambos saem com código 0 quando a skill está válida.

## Status do conteúdo

Nem todo número ou atribuição foi conferido na fonte primária. Os itens marcados como **[não verificado]** ou "segundo o autor" não devem ser citados como fato. A seção **Limites conhecidos** do `SKILL.md` lista o que ainda falta confirmar.

Partes de origem não verificada, mencionadas em `references/12`: as atribuições e opiniões de Rony Meisler e Alfredo Soares foram extraídas de um compilado de vídeos.

## Licença

Sem licença definida. O conteúdo é uma síntese de materiais de terceiros; confira as fontes antes de redistribuir.

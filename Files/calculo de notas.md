# Cálculo

## Mestrado

### Etapas do ingresso

- **Primeira etapa:** Nota do Pré-Projeto de Pesquisa (NPP)
  - Nota de 0 a 100; com 60 como nota mínima
- **Segunda etapa:** Análise de Formação Acadêmica e CV (NFA)
  1. Nota de Formação Acadêmica (NFA)
     1. Média do histórico escolar da graduação (NPP)
     2. Cursos de formação (MH)
     3. Prêmios (NCF)
     4. POSCOMP (PR)
  2. Nota de Currículo Vitae (NCV)
     1. Publicações em periódicos e eventos (PUB)
     2. Iniciação Científica (LI)
     3. Estágios (EAC?)
     4. Experiência profissional (EP)

| Etapa | Cat 1 | Critério | Peso  | Verbose                                 |
| ----- | ----- | -------- | ----- | --------------------------------------- |
| 1     | NPP   | NPP      | 0.4   | Nota do Pré-Projeto de Pesquisa         |
| 2     | NFA   | MH       | 0.125 | Média do histórico escolar da graduação |
| 2     | NFA   | NCF      | 0.025 | Cursos de formação                      |
| 2     | NFA   | PR       | 0.05  | Prêmios                                 |
| 2     | NFA   | PC       | 0.05  | POSCOMP                                 |
| 2     | NCV   | EP       | 0.05  | Experiência profissional                |
| 2     | NCV   | EAC      | 0.1   | Experiência Acadêmico-Científica        |
| 2     | NCV   | PUB      | 0.15  | Publicações                             |
| 2     | NCV   | LI       | 0.05  | Língua inglesa                          |

- $Nota\ Final = (NPP \cdot 0.4) + (NFA \cdot 0.6) + (NCV \cdot 0.6)$
  - $NPP = Introdução \cdot 0.3 + Referencial\ Teórico \cdot 0.3 + Metodologia \cdot 0.1 + Cronograma \cdot 0.1 + Clareza \cdot 0.2$
  - $NFA = MH \cdot 0.125 + NCF \cdot 0.025 + PR \cdot 0.05 + PC \cdot 0.05$
    - $MH = Histórico\ Graduação \cdot 0.4 + Histórico\ Pós-Graduação \cdot 0.4 + Cursos\ extracurriculares \cdot 0.2$
    - $NCF = Cursos\ de\ formação$
    - $PR = Prêmios$
    - $PC = POSCOMP$
  - $NCV = EP \cdot 0.05 + EAC \cdot 0.1 + PUB \cdot 0.15 + LI \cdot 0.05$
    - $EP = Experiência\ profissional$
    - $EAC = Experiência\ Acadêmico-Científica$
    - $PUB = Publicações$
    - $LI = (A1, A2, B1, B2, C1, C2) = (0, 5, 25, 50, 100, 100)$

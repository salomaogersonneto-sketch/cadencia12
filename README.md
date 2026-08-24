# Cadência 12

Programa de 12 semanas de bike indoor (spinning em casa) com aula guiada bloco a bloco, ofensiva diária estilo Duolingo e acompanhamento de VO₂ estimado.

**App no ar:** https://salomaogersonneto-sketch.github.io/cadencia12/

## O que tem dentro

- **Hoje** — sessão do dia, ofensiva, XP, nível e a semana inteira em um cartão.
- **Aula guiada** — player em tela cheia com cronômetro por bloco, RPM alvo, resistência, posição na bike, faixa de FC calculada da sua FCmáx, bipe de transição e trava de tela.
- **Programa** — as 12 semanas em 3 blocos (Base + VO₂, Limiar + VO₂, Pico), com deload e teste marco nas semanas 4, 8 e 12.
- **Progresso** — minutos por semana, kcal acumuladas, 15 medalhas e a tabela dos testes marco com VO₂ estimado.
- **Perfil** — peso, idade, FCmáx, FC de repouso, data de início e a calibração da escala de resistência R2–R7.

## Estrutura da semana

| Dia | Sessão |
|---|---|
| Seg | VO₂ Norueguês (4–6 × 4 min) |
| Ter | Base Aeróbica em Z2 |
| Qua | Escalada Sweet Spot / Limiar 2×18 |
| Qui | Recuperação Ativa |
| Sex | Queima 40/20 |
| Sáb | Longo com surtos |
| Dom | Ativa + mobilidade |

## Como usar

Abra o link no celular e adicione à tela de início (**Compartilhar → Adicionar à Tela de Início** no iPhone, **Instalar app** no Android). Ele funciona sem internet depois da primeira abertura.

Os dados ficam salvos no navegador do próprio aparelho (`localStorage`). Trocar de celular ou limpar os dados do site apaga o histórico — use **Perfil → Exportar JSON** para guardar uma cópia.

## Detalhes técnicos

Uma página HTML sem dependências, sem build e sem backend. Único recurso externo: Google Fonts (Archivo, IBM Plex Sans, IBM Plex Mono).

- Zonas por %FCmáx, com FCmáx estimada por Tanaka (208 − 0,7 × idade) quando não medida.
- Calorias por MET × 3,5 × peso ÷ 200, somadas bloco a bloco.
- VO₂ estimado por 15,3 × (FCmáx ÷ FC de repouso). Serve para tendência, não é valor de laboratório.

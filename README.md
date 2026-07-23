# Auditorias-SHEE-

Ferramentas internas do grupo de farmácias **SHEE**.

## Portal Performance de Equipas

`Portal Performance Equipas.html` — portal para avaliar a performance das equipas ao longo
do tempo, a partir dos dados exportados do **Sifarma.Gest**. Reproduz os indicadores do
relatório mensal de Recursos Humanos da ANF, mas de forma interativa e com histórico
(evolutivo e acumulado por **mês, trimestre, semestre e ano**).

### Como usar
1. Abrir o ficheiro `Portal Performance Equipas.html` no navegador (duplo clique).
2. Arrastar para a página o ficheiro **«dados operadores»** exportado do Sifarma.Gest
   (formato `.txt`, separado por `;`). Pode conter vários meses — cada importação atualiza
   os meses correspondentes sem apagar o histórico anterior.
3. Escolher o período (Mês / Trimestre / Semestre / Ano / Acumulado YTD) na barra superior.
   Cada período é comparado automaticamente com o período anterior ou homólogo.

### Vistas
- **Resumo** — KPIs do período (vendas, margem, atendimentos, venda/atendimento,
  margem/atendimento) com variação, e evolução mensal de todos os indicadores.
- **Equipa** — ranking de colaboradores com variação de posição, gráficos de % de
  atendimentos, venda/atendimento e margem/atendimento vs média da farmácia. Exportável para CSV.
- **Evolutivo Colaborador** — evolução individual de cada colaborador vs média da farmácia.
- **Grandes Mercados** — composição MSRM / MNSRM / PSBE / Outros por colaborador.
- **Genéricos** — top laboratórios do período (genéricos destacados), vendas de genéricos por
  colaborador (Generis, Viatris, Teva, KRKA, Tecnimede, …) e evolução da percentagem de genéricos.
  É um indicador **por laboratório** — não substitui a «% de Genéricos em Grupos Homogéneos» da ANF,
  que exige a marcação de genérico ao nível do produto (não disponível neste export).
- **Acumulados** — comparação trimestral, semestral e homóloga (ano vs ano).

> As **Avaliações de Desempenho** (slides 7 e 13 do relatório da ANF) não constam do export
> «dados operadores» — vêm de outro domínio do Sifarma. Ficam por integrar caso esses dados
> sejam disponibilizados.

### Notas
- Os dados ficam guardados **apenas no navegador** (localStorage). Nada é enviado para a internet.
- O botão **Gerir** permite ver, remover um mês específico ou apagar todos os dados.
- Os valores foram validados contra o relatório da ANF (vendas, margem, atendimentos,
  venda/atendimento, margem/atendimento e grandes mercados coincidem ao euro).

## Checklist Auditoria Farmácias

`Checklist Auditoria Farmácias 2026.html` — plano de ação e checklist de auditoria às farmácias.

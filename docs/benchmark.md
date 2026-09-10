# Benchmark de soluções existentes

Foram analisadas três soluções que ajudam a organizar compromissos ou registrar
tempo. A comparação considera o problema específico do Plantão Legal e não presume
que alguma delas seja uma solução clínica. As páginas foram consultadas em 10 de
setembro de 2026.

## 1. Google Calendar

- **Principais funcionalidades:** criação de eventos, recorrência, lembretes,
  visualização por dia/semana/mês e compartilhamento de agendas.
- **Pontos positivos:** interface conhecida, boa visualização temporal, lembretes e
  integração com outros serviços.
- **Pontos negativos:** exige configuração manual para transformar cada plantão em
  evento; não calcula horas extras de modo específico nem oferece indicador de fadiga.
  O compartilhamento pode ser inadequado para dados sensíveis de jornada.
- **Interface/experiência:** calendário visual e flexível, porém com mais etapas do
  que o desejável para registrar rapidamente um plantão já encerrado.
- **Fonte:** [Google Calendar](https://calendar.google.com/).

## 2. Toggl Track

- **Principais funcionalidades:** cronômetro de tempo, lançamentos manuais,
  projetos, etiquetas, relatórios e exportação.
- **Pontos positivos:** detalhamento de tempo, relatórios úteis e possibilidade de
  corrigir lançamentos manualmente.
- **Pontos negativos:** é orientado à produtividade e faturamento, não à recuperação
  entre plantões; a configuração de projetos e categorias pode aumentar o esforço de
  uso; não possui indicador preventivo de fadiga específico.
- **Interface/experiência:** registro por cronômetro é direto durante a atividade,
  mas pode falhar quando o usuário esquece de iniciar ou parar o contador.
- **Fonte:** [Toggl Track](https://toggl.com/track/).

## 3. WorkingHours

- **Principais funcionalidades:** registro de períodos trabalhados, metas, saldo de
  horas, estatísticas, temporizador e exportação de dados.
- **Pontos positivos:** foco em acompanhamento de horas, suporte a múltiplos
  empregos e visualização de saldo; aproxima-se do problema de jornada variável.
- **Pontos negativos:** não foi desenhado especificamente para plantões críticos,
  descanso ou fadiga; a quantidade de opções pode pesar para quem só precisa registrar
  rapidamente um turno; os recursos variam conforme plataforma e versão.
- **Interface/experiência:** concentra informações de tempo e saldo, mas o Plantão
  Legal pode ser mais objetivo ao destacar descanso, horas extras e privacidade local.
- **Fonte:** [WorkingHours](https://workinghoursapp.com/).

## O que pode ser aproveitado ou melhorado

Podemos aproveitar do Google Calendar a visualização por períodos e os lembretes; do
Toggl Track, os lançamentos manuais e relatórios; e do WorkingHours, o saldo de horas
e a separação por vínculo. O projeto deve reduzir a configuração inicial, permitir
registro offline em até três interações, calcular automaticamente duração e extras,
mostrar um indicador preventivo de carga e manter os dados sob controle local do
usuário.

## O que o aplicativo poderá fazer de diferente ou melhor?

O Plantão Legal será específico para profissionais de plantão: reunirá registro
rápido, histórico, cálculo de horas extras, acompanhamento do descanso e indicador de
fadiga em uma experiência curta e privada. O diferencial não será diagnosticar o
usuário, mas transformar registros simples de jornada em uma visão preventiva e
compreensível, funcionando sem internet e exportando relatórios somente quando o
usuário decidir.
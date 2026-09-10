# Pesquisa: jornada de trabalho e fadiga

## Objetivo

Esta pesquisa investiga o problema enfrentado por profissionais que trabalham em
plantões ou jornadas variáveis. O foco é entender como carga horária, descanso,
fadiga e privacidade devem influenciar o Plantão Legal. As fontes foram consultadas
em 10 de setembro de 2026.

## Achados da pesquisa

### Jornadas extensas aumentam riscos

O NIOSH relaciona jornadas longas e trabalho em turnos a mais fadiga, menor tempo
de recuperação e maior risco de erros e acidentes. A orientação também destaca a
importância de pausas e de períodos adequados de descanso. Para o aplicativo, isso
reforça a necessidade de registrar início, término, horas extras e intervalo de
descanso de forma rápida, além de mostrar a carga acumulada com linguagem de alerta,
sem afirmar que o usuário possui uma condição clínica.

### Burnout é um fenômeno ocupacional

A Organização Mundial da Saúde classifica burnout na CID-11 como fenômeno
ocupacional resultante de estresse crônico no trabalho não gerenciado com sucesso.
Isso não transforma o aplicativo em instrumento de diagnóstico. O produto deve
apoiar percepção e organização da jornada, indicar sobrecarga de forma preventiva e
orientar o usuário a procurar apoio profissional ou institucional quando necessário.

### Registros precisam funcionar em contexto real

Profissionais de saúde, segurança, transporte e emergência podem estar cansados,
em ambientes com ruído, conectividade instável ou pouco tempo disponível. Um fluxo
com poucos campos, confirmação clara e uso offline reduz o risco de deixar o registro
para depois. A pesquisa da ILO sobre tempo de trabalho também evidencia que o
acompanhamento de horas e períodos de descanso é relevante para condições de trabalho
mais seguras e equilibradas.

### Dados de jornada exigem privacidade

Horários, locais e padrões de trabalho podem revelar informações profissionais
sensíveis. A coleta deve ser mínima e o usuário deve controlar exportação, exclusão e
compartilhamento. Por isso, o projeto prevê armazenamento local, sincronização apenas
por Wi-Fi e geração de PDF sob ação explícita do usuário.

## Três descobertas importantes e impacto no projeto

1. **A fadiga é influenciada por duração e recuperação, não apenas pelo total de
   horas.** O painel deverá combinar carga acumulada, horas extras e tempo desde o
   último plantão, incentivando descanso sem produzir diagnóstico.
2. **O momento do registro é crítico: pode ocorrer após uma jornada cansativa.** O
   cadastro deve pedir somente data, início e término e ser concluído em até três
   interações, com funcionamento offline.
3. **Os dados podem expor a rotina profissional do usuário.** O aplicativo deverá
   priorizar armazenamento privado, permissões mínimas, exportação manual de PDF e
   exclusão controlada dos registros.

## Fontes

- World Health Organization. [Burn-out an occupational phenomenon](https://www.who.int/mental_health/evidence/burn-out/en/).
- CDC/NIOSH. [Long Work Hours, Extended or Irregular Shifts, and Worker Fatigue](https://www.cdc.gov/niosh/work-hour-training-for-nurses/longhours/mod7/05.html).
- International Labour Organization. [Working Time and Work-Life Balance Around the World](https://www.ilo.org/publications/working-time-and-work-life-balance-around-world).
- World Health Organization. [WHO guidelines on mental health at work](https://www.who.int/publications/i/item/9789240053052).
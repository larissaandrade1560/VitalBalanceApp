# Estudo de Caso - Plantão Legal

## 2.1 Problema

O trabalho em regime de plantão envolve jornadas variáveis, alternância de turnos e, em muitos casos, acúmulo de horas extras. Quando esses períodos não são registrados de forma sistemática, o trabalhador pode perder a percepção da própria carga horária, deixar de identificar insuficiência de descanso e ter dificuldades para conferir sua remuneração ou sua escala.

O Plantão Legal pretende solucionar essa dificuldade por meio do registro e do acompanhamento de plantões e horas extras em um único aplicativo. A solução deve permitir que o usuário informe rapidamente os horários trabalhados, utilize uma calculadora de carga horária, consulte o histórico, visualize um indicador de fadiga em formato de bateria e exporte relatórios em PDF.

Esse problema é relevante porque a exposição contínua a jornadas extensas e a períodos insuficientes de recuperação pode provocar fadiga, reduzir a atenção e comprometer a qualidade do trabalho. Em atividades como atendimento de saúde, segurança, transporte e combate a incêndios, a fadiga também pode ampliar riscos para terceiros. Além disso, a ausência de registros confiáveis enfraquece a capacidade do profissional de organizar sua rotina e de reconhecer sinais de sobrecarga antes que evoluam para burnout.

A necessidade principal atendida será o controle simples, rápido e privado da jornada. O aplicativo não substitui avaliação médica, orientação trabalhista ou políticas institucionais de saúde ocupacional; ele oferece ao usuário uma base organizada para acompanhar seus próprios dados e tomar decisões mais conscientes sobre descanso, disponibilidade e aceitação de horas adicionais.

## 2.2 Público e usuários

Os usuários do Plantão Legal são profissionais com jornadas fixas, variáveis ou distribuídas em diferentes locais de trabalho. O público inclui médicos, enfermeiros, técnicos de enfermagem, seguranças, motoristas de aplicativo e bombeiros. Embora suas atividades sejam distintas, esses grupos compartilham a necessidade de registrar períodos de trabalho que podem ocorrer fora de um horário comercial regular.

A relação dos usuários com o aplicativo é operacional e recorrente: eles utilizarão a solução para cadastrar um plantão, informar início e término da jornada, registrar horas extras e consultar o histórico. O uso tende a ocorrer antes do trabalho, para conferir a escala; durante ou logo após o plantão, para registrar horários com maior precisão; e em momentos de planejamento, para avaliar a carga acumulada e os períodos de descanso.

As necessidades variam conforme a atividade profissional:

- **Médicos, enfermeiros e técnicos de enfermagem:** precisam acompanhar escalas extensas, plantões consecutivos e horas adicionais em ambientes nos quais a fadiga pode afetar decisões e atendimento.
- **Seguranças e bombeiros:** necessitam controlar turnos prolongados e escalas alternadas, preservando a atenção necessária para situações de risco.
- **Motoristas de aplicativo:** precisam registrar períodos de conexão e trabalho flexíveis, nos quais a jornada não é necessariamente definida por uma escala formal.

Em todos os casos, a interação deve exigir pouco esforço cognitivo. O usuário provavelmente acessará o aplicativo em intervalos curtos, após uma jornada cansativa ou em ambientes com conectividade limitada. Por isso, o registro de um plantão deve ser direto, com dados essenciais e confirmação clara, enquanto a calculadora, o indicador em formato de bateria e os relatórios em PDF devem apoiar uma análise posterior mais detalhada.

## 2.7 Restrições e condições

As restrições definem um produto deliberadamente focado. Elas reduzem a complexidade da primeira versão e orientam decisões de interface, arquitetura, segurança e priorização funcional.

- **Até 4 telas principais:** a solução deve concentrar o fluxo em telas de painel, registro de plantão, histórico e relatórios/configurações. Essa limitação evita a fragmentação das tarefas e facilita a localização das funções mais utilizadas.
- **Funcionalidade principal em até 3 interações:** o cadastro de um plantão deve ser concluído em, no máximo, três etapas ou ações relevantes. Essa condição é essencial para uso após uma jornada cansativa e reduz o risco de registros incompletos.
- **Android 7.0 ou superior:** a aplicação deve considerar os recursos e as limitações de dispositivos compatíveis com essa versão. É necessário evitar depender exclusivamente de APIs recentes e testar diferentes tamanhos de tela e capacidades de hardware.
- **Registro rápido de plantões:** o fluxo deve solicitar apenas os dados essenciais, como data, início e término, calculando automaticamente a duração e permitindo identificar horas extras.
- **Calculadora de carga horária:** o aplicativo deve consolidar as horas trabalhadas e extras em períodos definidos, com critérios transparentes e sem presumir regras trabalhistas específicas para todos os usuários.
- **Indicador de fadiga em formato de bateria:** os níveis devem representar visualmente a carga acumulada e funcionar como alerta preventivo, sem caracterizar diagnóstico clínico.
- **Funcionamento offline:** o registro não pode depender de uma conexão ativa, pois o usuário pode estar em hospitais, áreas operacionais, estacionamentos ou outros locais com sinal instável. Os dados devem ser salvos localmente e permanecer disponíveis para consulta.
- **Sincronização somente por Wi-Fi:** quando houver sincronização, ela deve ocorrer apenas em redes Wi-Fi, mediante uma condição verificável pelo sistema. Essa regra reduz o consumo de dados móveis e exige que o aplicativo informe claramente quando existem registros pendentes.
- **Exportação de relatórios PDF locais:** os relatórios de jornada devem ser gerados e armazenados no próprio dispositivo, sem envio automático para um servidor. O usuário deve conseguir localizar o arquivo e controlar seu compartilhamento.
- **Foco em modo noturno:** a interface deve priorizar baixo brilho, contraste adequado e leitura confortável em ambientes escuros. O modo noturno não deve reduzir a legibilidade nem ocultar estados importantes, especialmente em telas de acompanhamento.
- **Privacidade dos dados de jornada:** horários, locais e padrões de trabalho podem revelar informações profissionais sensíveis. A coleta deve ser limitada ao necessário, sem exposição pública ou compartilhamento automático, e o usuário deve ter controle sobre exportação e exclusão.
- **Notificações locais:** alertas de descanso, registros pendentes ou carga horária elevada devem ser processados no dispositivo. As notificações precisam ser configuráveis para não se transformarem em fonte adicional de interrupção ou ansiedade.
- **Armazenamento local seguro:** os dados devem ser protegidos contra acesso indevido no dispositivo, usando mecanismos apropriados da plataforma, como armazenamento privado do aplicativo e, quando disponível, criptografia. Também é necessário tratar falhas de gravação e evitar perda silenciosa dos registros.

Essas condições apresentam um equilíbrio entre utilidade e viabilidade acadêmica. O escopo offline e local reduz dependências de infraestrutura, mas transfere para o aplicativo a responsabilidade de garantir consistência, recuperação e proteção dos dados. Da mesma forma, limitar a quatro telas favorece a simplicidade, porém exige uma arquitetura de informação rigorosa para que relatórios, alertas e registros não concorram pela atenção do usuário.

## 2.8 Pontos de atenção

### 1. Registro rápido e confiável da jornada

O valor central do Plantão Legal depende da qualidade dos dados registrados. Se cadastrar um plantão for demorado, exigir conexão ou apresentar campos confusos, o usuário poderá adiar o registro e comprometer a precisão do histórico. O fluxo em até três interações deve priorizar data, horário de início, horário de término e identificação de horas extras, permitindo complementações posteriores quando necessário. Também devem existir validações para horários inválidos, jornadas incompletas e sobreposição de registros.

### 2. Segurança e privacidade dos dados pessoais

O aplicativo armazena informações que podem expor rotinas profissionais e padrões de disponibilidade. Uma falha de privacidade pode gerar consequências mais graves do que a simples perda de conveniência, especialmente para trabalhadores que atuam em locais sensíveis ou acumulam vínculos. O armazenamento local seguro, o controle de exportação dos PDFs e a ausência de sincronização em redes móveis devem ser tratados como requisitos de produto, e não apenas como detalhes de implementação. A interface também deve comunicar estados de sincronização e compartilhamento sem ambiguidades.

### 3. Indicador preventivo e proteção dos dados

A missão de prevenir fadiga extrema e burnout exige um indicador de bateria útil, mas o aplicativo não deve apresentar conclusões clínicas ou criar uma falsa sensação de segurança. Os níveis devem ser baseados em limites configuráveis e padrões de carga horária, com linguagem objetiva e não alarmista. Paralelamente, os dados de jornada devem permanecer protegidos no armazenamento local, e os relatórios PDF só devem ser compartilhados mediante ação explícita do usuário. É importante distinguir um aviso de atenção de um diagnóstico, incentivar pausas e descanso e deixar claro que situações de sofrimento ou risco exigem apoio profissional e institucional. Essa abordagem preserva o foco preventivo do projeto sem ultrapassar seus limites acadêmicos e funcionais.

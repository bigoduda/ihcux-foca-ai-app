FocaAí — Protótipo de Baixa Fidelidade (IHC & UX)
Protótipo de baixa fidelidade para o aplicativo FocaAí, sistema de gestão de foco baseado nos princípios de Calm Technology. O app combina Pomodoro, bloqueio seletivo de aplicativos, jardim digital (árvore virtual), métricas de tempo ganho e sessões de foco em grupo — tudo sem gerar ansiedade ou vício.

👤 Integrante
Eduarda Luiza Vitorio — RA: 326135721
📱 Telas do Protótipo
O protótipo contém 6 telas principais desenhadas em estilo wireframe monocromático, com espaço negativo superior a 60% em cada tela:

Nº	Tela	Função
01	Seleção de Ambiente	Escolha de som (chuva, café, floresta, silêncio) e tempo de foco via slider
02	Configuração de Bloqueio	Lista minimalista de apps com toggles on/off
03	Dashboard / Foco Ativo	Timer circular central, árvore que cresce, botão de pausa
04	Sala em Grupo	Lista de amigos focando juntos, tempo coletivo, sem ranking competitivo
05	Relatório de Conquistas	"Tempo ganho para a vida" (não "tempo de tela"), gráfico semanal, floresta plantada
06	Tentativa de Saída	Aviso suave de que a árvore "vai morrer", sem cor de alarme, sem barreira física
🌿 Conceito de Design — Calm Technology como antídoto à ansiedade
A pergunta central do projeto não foi "como prender o usuário no app?", mas "como construir uma interface que respeite o estado emocional de quem está tentando focar?". A resposta veio dos princípios de Mark Weiser e Amber Case sobre Calm Technology, traduzidos em decisões concretas:

O que NÃO existe na interface (e por quê)
Sem vermelho, sem laranja, sem amarelo. Cores de alarme ativam o sistema nervoso simpático — exatamente o oposto do que um app de foco deveria fazer. Toda a paleta é monocromática.
Sem números piscando ou contagens regressivas dramáticas. O timer central é finíssimo, em peso 200. Ele informa, não pressiona.
Sem badges, sem streaks, sem notificações. Streaks de Duolingo geram ansiedade quando quebram. O FocaAí não tem essa armadilha emocional: cada sessão é completa em si mesma.
Sem ranking competitivo na sala em grupo. A tela 04 mostra apenas o status de cada amigo. Ninguém é "primeiro lugar". Quando alguém pausa, aparece "pausou" em cinza — não há emoji triste, não há culpa visual.
Sem métricas que culpam. "Tempo de tela" foi reformulado como "tempo ganho para a vida". A mesma informação, mas posicionada como ganho, não como perda.
O que EXISTE para gerar calma
Espaço negativo dominante. Cada tela tem mais espaço vazio do que conteúdo. O olho descansa.
Tipografia leve (pesos 100–300). O texto sussurra. Os números grandes do timer são pesados visualmente apenas pela escala, não pela espessura.
Hierarquia de um só centro. Há apenas um elemento grande por tela: o tempo restante, o gráfico, ou a mensagem da árvore. Nenhuma competição visual.
Respiração no fundo. Durante a sessão ativa, o fundo pulsa lentamente (ciclo de 10s, sincronizado com respiração diafragmática). Indução fisiológica de calma — uma sugestão sensorial à beira da atenção, exatamente como Weiser preconiza.
Saída sem barreira. A tela 06 não bloqueia. A árvore "morre" como consequência simbólica, mas o botão "Sair mesmo assim" é texto sublinhado simples — não tem cor de aviso, não tem confirmação dupla. O usuário sempre pode sair. Respeito é a métrica final.
"O melhor design é aquele que faz o usuário guardar o celular e olhar para o mundo." — A interface comunica que está tudo bem em se desconectar literalmente nas três últimas microinterações do fluxo: a saída não é punida, a pausa não é envergonhada, e o app não envia notificações para "te trazer de volta".

🔄 Fluxo de Usuário — Sessão de Foco em Grupo
[01] CONVITE
      │  Amigo compartilha link da sala via mensagem
      ▼
[02] AMBIENTE
      │  Escolhe som (Chuva selecionada por padrão)
      │  Arrasta slider para definir 30 min
      ▼
[03] BLOQUEIO
      │  Confirma os 3 apps já marcados (Instagram, TikTok, Twitter)
      │  Pode adicionar mais com o "+"
      ▼
[04] FOCO ATIVO  ◀━━ tela central
      │  Timer circular, árvore crescendo
      │  Sala em grupo acessível por gesto lateral
      │  Fundo respira a 6 ciclos/min
      ▼
[05] CONCLUSÃO
      │  Árvore plantada na floresta
      │  Som de finalização suave (sino tibetano, não alarme)
      ▼
[06] RELATÓRIO
         "Você ganhou 30 minutos para a vida real"
         Gráfico semanal atualizado
Total: 4 toques para sair da configuração e estar focando com o grupo. O caminho é curto porque o atrito deve estar em outro lugar — não em começar a focar, mas em parar antes da hora.

🎚 Escolha de Componentes — Por que cada controle é o que é
Por que slider, não input numérico, para o tempo de foco?
Definir tempo de foco não é uma decisão racional — é um gesto corporal de compromisso. Digitar "47 minutos" coloca o usuário em modo planejamento ansioso ("será que dá tempo?"). Arrastar um slider entre 15 e 90 min é tátil, aproximado, gentil. Os valores marcados (15, 30, 45, 60, 90) são socialmente reconhecidos como blocos de foco saudáveis — o slider naturalmente conduz a escolhas razoáveis sem precisar restringir.

Por que toggles, não checkboxes, na lista de apps?
Toggles comunicam estado binário ativo agora. Checkboxes comunicam seleção para confirmação futura. Como o bloqueio é instantâneo (assim que o toggle vira, o app está bloqueado), a linguagem visual precisa transmitir essa imediatez. Além disso, toggles têm uma área de toque mais generosa e um feedback háptico mais satisfatório.

Por que cards de som com onda visual em vez de ícones?
Cada card tem uma mini-representação da textura sonora (▁▂▃▂▁ para chuva, · para silêncio). Ícones de "🌧️" ou "☕" estariam carregados emocionalmente e exigiriam interpretação cultural. As ondas são abstratas, calmas, e comunicam intensidade relativa.

Por que botão de pausa, não de parar, na tela de foco?
A linguagem importa. "Pausar" preserva a sessão e a árvore. "Parar" sugere desistência. Internamente, o sistema permite retomar até por 2 minutos antes de considerar a sessão encerrada — o usuário pode ir ao banheiro sem perder a árvore. Isso reflete realidade humana sem premiar abandono.

Por que avatares circulares com inicial em vez de fotos de perfil?
Fotos de perfil em uma sala de foco geram dois ruídos: comparação social (todo mundo está focado, "eu também devia estar produzindo") e curiosidade visual ("ah, o Pedro mudou a foto, deixa eu olhar"). Iniciais em P&B removem completamente esses gatilhos.

🌒 Desafios Extras
Modo Noturno Extremo (planejado)
Versão da interface apenas com contornos finíssimos sobre fundo preto puro (#000), sem nenhum pixel branco preenchido. Em telas OLED isso economiza ~60% da bateria e elimina a emissão de luz azul. Tipografia em peso 100, sem áreas de cor sólida. Os toggles ativos viram contornos preenchidos por um único pixel de borda. Pensado para sessões de foco noturnas onde o usuário não quer que o app contribua para insônia.

Acessibilidade para usuários com TDAH
A organização visual do FocaAí beneficia diretamente quem tem TDAH por três motivos estruturais:

Um elemento foco-grande por tela elimina a paralisia de decisão que aparece quando há múltiplos estímulos competindo. Em qualquer momento, o cérebro sabe onde olhar.
Ausência de notificações push e badges remove os principais gatilhos de hiperfocalização forçada e quebra de fluxo. O app não chama o usuário — o usuário escolhe quando voltar.
Linguagem visual de "ganho", não de "déficit". Mostrar "8h ganhas para a vida" em vez de "você passou 4h no Instagram" remove a vergonha que tipicamente faz pessoas com TDAH abandonarem apps de produtividade. A sensação é de jogo cooperativo consigo mesmo, não de fiscalização externa.
A respiração do fundo também atua como âncora sensorial passiva — um padrão rítmico que pode ajudar a regular atenção sem exigir esforço consciente.

🛠 Ferramentas e Entrega
Prototipagem: planejada no Miro; este repositório contém a exportação final.
Estilo: wireframe de baixa fidelidade, preto e branco, com espaço negativo dominante.
Arquivos entregues:
/prototipo/prototipo.png — captura em alta resolução do board completo
/prototipo/prototipo.pdf — versão em PDF para impressão e revisão
💭 Reflexão de UX
"Muitas vezes, o melhor design é aquele que faz o usuário guardar o celular e olhar para o mundo. Como o seu protótipo comunica que 'está tudo bem em se desconectar'?"

Resposta: o FocaAí comunica isso em três níveis simultâneos.

Visual: a interface inteira é tão silenciosa que o próprio celular já parece menos presente. Pouco brilho, pouca informação, pouca cor. O dispositivo se aproxima de um objeto inerte.

Comportamental: o app não pune saídas. A tela 06 mostra a consequência (árvore morre), mas o botão de sair existe, é acessível, e não tem cor de aviso. O usuário pode sair a qualquer momento, e o app aceita isso. Quando a sessão termina com sucesso, não há fogos de artifício digitais — apenas um som suave e um número atualizado. A celebração não vicia.

Linguístico: a métrica final não é "tempo no app", é "tempo ganho para a vida". O sucesso do app é, por definição, o usuário não usando o celular. É um app que torce contra si mesmo. E essa é, talvez, a única honestidade possível para uma tecnologia de foco.

**Comece com o Windows**  
Permite iniciar o RivaTuner Statistics Server com o Windows. Habilite esta opção somente ao usar o RivaTuner Statistics Server como uma solução autônoma de monitoramento de taxa de quadros. Se você estiver usando este aplicativo em conjunto com clientes como RivaTuner, HIS iTurbo, EVGA Precision ou MSI Afterburner, os clientes carregarão o servidor quando necessário.  
*Dicas:*  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Mostrar exibição na tela**  
Controla globalmente a visibilidade do On-Screen Display. Use esta opção para ocultar o On-Screen Display sem alterar os perfis. Os aplicativos cliente também podem controlar remotamente esta opção por meio de teclas de atalho.  
*Dicas:*  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Nível de detecção de aplicativo: Nenhum**  
Desabilita a detecção para o aplicativo associado ao perfil atual. Neste modo, o RivaTuner Statistics Server não coleta estatísticas de tempo de execução, como taxa de quadros, e não fornece serviços adicionais, como On-Screen Display, para o aplicativo associado.  
*Dicas:*  
- Alguns aplicativos protegidos podem tratar o hooking de código executável, necessário para a detecção adequada do aplicativo, coleta de estatísticas e renderização do On-Screen Display, como uma possível ameaça e se recusar a executar. Para solucionar esses problemas, tente adicionar um perfil para esse aplicativo e diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Nível de detecção do aplicativo: baixo**  
Seleciona um nível de detecção baixo para o aplicativo associado ao perfil atual. Neste modo, o RivaTuner Statistics Server intercepta as chamadas do aplicativo para bibliotecas de tempo de execução Direct3D e OpenGL. Este modo é recomendado para coletar estatísticas de tempo de execução, como taxa de quadros, e habilitar serviços adicionais, como On-Screen Display, na maioria dos aplicativos 3D modernos.  
*Dicas:*  
- Alguns aplicativos protegidos podem tratar o hooking de código executável, necessário para a detecção adequada do aplicativo, coleta de estatísticas e renderização do On-Screen Display, como uma possível ameaça e se recusar a executar. Para solucionar esses problemas, tente adicionar um perfil para esse aplicativo e diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Nível de detecção do aplicativo: médio**  
Seleciona um nível de detecção médio para o aplicativo associado ao perfil atual. Neste modo, o RivaTuner Statistics Server intercepta as chamadas do aplicativo para as bibliotecas de tempo de execução DirectDraw, Direct3D e OpenGL. Este modo é recomendado para coletar estatísticas de tempo de execução, como taxa de quadros, e habilitar serviços adicionais, como On-Screen Display, na maioria dos aplicativos 3D modernos, bem como em aplicativos que usam interfaces de aceleração de hardware 2D/3D desatualizadas, como DirectDraw e Direct3D7.  
*Dicas:*  
- Alguns aplicativos protegidos podem tratar o hooking de código executável, necessário para a detecção adequada do aplicativo, coleta de estatísticas e renderização do On-Screen Display, como uma possível ameaça e se recusar a executar. Para solucionar esses problemas, tente adicionar um perfil para esse aplicativo e diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Nível de detecção do aplicativo: alto**  
Seleciona um alto nível de detecção para o aplicativo associado ao perfil atual. Neste modo, o RivaTuner Statistics Server intercepta as chamadas do aplicativo para bibliotecas de tempo de execução DirectDraw, Direct3D e OpenGL e intercepta as tentativas do aplicativo de carregar novas bibliotecas. Este modo é recomendado para coletar estatísticas de tempo de execução, como taxa de quadros, e habilitar serviços adicionais, como On-Screen Display, em aplicativos que carregam bibliotecas de tempo de execução DirectDraw, Direct3D e OpenGL dinamicamente.  
*Dicas:*  
- Alguns aplicativos protegidos podem tratar o hooking de código executável, necessário para a detecção adequada do aplicativo, coleta de estatísticas e renderização do On-Screen Display, como uma possível ameaça e se recusar a executar. Para solucionar esses problemas, tente adicionar um perfil para esse aplicativo e diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Modo furtivo**  
Os sistemas anti-cheat de alguns jogos podem tratar o hooking de código de jogo, necessário para detecção de aplicativos e renderização On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Habilitar o modo stealth pode ajudar a resolver esses problemas. Quando esse modo é habilitado, o RivaTuner Statistics Server usa técnicas sofisticadas de hooking de código, dificultando que aplicativos de terceiros detectem o hook.  
*Dicas:*  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Suporte Direct3D personalizado: Habilitar compatibilidade com bibliotecas de tempo de execução Direct3D modificadas**  
Por padrão, o RivaTuner Statistics Server suporta aplicativos Direct3D usando somente bibliotecas nativas de tempo de execução do Microsoft Direct3D. Você pode habilitar esta opção para torná-la compatível com aplicativos Direct3D usando bibliotecas proxy Direct3D de tempo de execução modificadas personalizadas (por exemplo, aplicativos Direct3D habilitados para InjectFXAA). Esta opção é específica do perfil, então você pode configurá-la independentemente para diferentes aplicativos. Não é recomendado habilitá-la globalmente, pois o modo de compatibilidade pode impedir que alguns aplicativos Direct3D sejam iniciados.  
*Dicas:*  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Limite de taxa de quadros**  
Permite alternar entre os modos de limite de framerate e frametime. No modo frametime, o limite é especificado como o frametime alvo com precisão de 1 microssegundo.  
*Dicas:*  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Modo de sincronização de linha de varredura**  
Permite alternar entre os modos de sincronização de linha de varredura simples, dupla e meia. No modo de sincronização de linha de varredura simples, a taxa de quadros é sincronizada com a posição do rasterizador a cada período de atualização do display. Em outras palavras, você está limitando a taxa de quadros à taxa de atualização e obtendo um efeito VSync ON com uma linha de ruptura localizada em uma posição fixa. A linha de ruptura pode ser movida para baixo e oculta no intervalo de apagamento vertical. No modo de sincronização de linha de varredura dupla, a taxa de quadros é sincronizada com a posição do rasterizador duas vezes por período de atualização do display. Em outras palavras, você está limitando a taxa de quadros ao dobro da taxa de atualização e obtendo um efeito VSync ON com duas linhas de ruptura localizadas em posições fixas. Ambas as linhas de ruptura podem ser movidas para baixo e uma delas pode ser oculta no intervalo de apagamento vertical. No modo de sincronização de meia linha de varredura, a taxa de quadros é sincronizada com a posição do rasterizador uma vez a cada dois períodos de atualização do display. Em outras palavras, você está limitando a taxa de quadros à metade da taxa de atualização e obtendo um efeito VSync ON com uma linha de ruptura localizada em uma posição fixa. Nesse caso, a linha de ruptura pode ser movida para baixo e escondida no intervalo de obturação vertical.  
*Dicas:*  
- É necessário desabilitar o VSync para uma funcionalidade adequada de sincronização da linha de varredura.  
- Você pode habilitar a sincronização de scanline em conjunto com os modos de limitação de taxa de quadros de sincronização de borda frontal/traseira para ativar os modos de sincronização de scanline híbridos. Neste caso, a sincronização real da scanline alvo é realizada apenas uma vez no início da limitação de taxa de quadros, e então você pode direcionar o posicionamento da tearline com o relógio do sistema.  
- Você pode usar a sobreposição do FCAT no modo de barra móvel como um indicador visual da posição da linha de ruptura.  
- Você pode especificar um índice de linha de varredura negativo para definir o deslocamento do número total de linhas de varredura.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Habilitar suporte para exibição na tela**  
Habilita o suporte de exibição na tela para o aplicativo associado ao perfil atual.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Exibição na tela: Modo de renderização vetorial 2D**  
O On-Screen Display pode ser renderizado usando fontes vetoriais ou raster via funções DirectX/OpenGL 2D aceleradas por hardware ou 3D aceleradas por hardware. A implementação baseada em aceleração 2D fornece compatibilidade máxima com a maioria dos mecanismos 3D de jogos existentes; no entanto, não é suportada em DirectX 10 e jogos mais recentes quando o antialiasing multiamostrado está habilitado. A aceleração 2D também pode ser mal otimizada em alguns drivers de vídeo, então a implementação baseada em aceleração 3D pode ser muito mais eficaz em termos de desempenho em tais sistemas. No entanto, a implementação 3D tem uma chance maior de ser incompatível com alguns mecanismos 3D de jogos. Tente desabilitar o modo 3D se notar alguma anomalia de renderização em um jogo ao executá-lo com o OSD habilitado.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Exibição na tela: Modo de renderização vetorial 3D**  
O On-Screen Display pode ser renderizado usando fontes vetoriais ou raster via funções DirectX/OpenGL 2D aceleradas por hardware ou 3D aceleradas por hardware. A implementação baseada em aceleração 2D fornece compatibilidade máxima com a maioria dos mecanismos 3D de jogos existentes; no entanto, não é suportada em DirectX 10 e jogos mais recentes quando o antialiasing multiamostrado está habilitado. A aceleração 2D também pode ser mal otimizada em alguns drivers de vídeo, então a implementação baseada em aceleração 3D pode ser muito mais eficaz em termos de desempenho em tais sistemas. No entanto, a implementação 3D tem uma chance maior de ser incompatível com alguns mecanismos 3D de jogos. Tente desabilitar o modo 3D se notar alguma anomalia de renderização em um jogo ao executá-lo com o OSD habilitado.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Exibição na tela: Modo de renderização 3D raster**  
O On-Screen Display pode ser renderizado usando fontes vetoriais ou raster via funções DirectX/OpenGL 2D aceleradas por hardware ou 3D aceleradas por hardware. A implementação baseada em aceleração 2D fornece compatibilidade máxima com a maioria dos mecanismos de jogos 3D existentes; no entanto, não é suportada no DirectX 10 e jogos mais recentes quando o antialiasing multiamostrado está habilitado. A aceleração 2D também pode ser mal otimizada em alguns drivers de vídeo, então a implementação baseada em aceleração 3D pode ser muito mais efetiva em termos de desempenho em tais sistemas. No entanto, a implementação 3D tem uma chance maior de ser incompatível com alguns mecanismos de jogos 3D. Tente desabilitar o modo 3D se notar alguma anomalia de renderização em um jogo enquanto o executa com o OSD habilitado. Você pode clicar no botão do modo de renderização 3D raster selecionado novamente para alterar o tipo e o estilo da fonte, ou segurar *Ctrl* e clicar novamente para carregar uma fonte raster pré-renderizada de um arquivo bitmap.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Espaço de coordenadas de exibição na tela: Viewport**  
Por padrão, o espaço de coordenadas do On-Screen Display corresponde ao espaço de coordenadas da viewport de renderização, ou seja, a última área retangular para a qual o aplicativo estava renderizando. No entanto, certos aplicativos (por exemplo, StarCraft II: Wings of Liberty) podem usar várias viewports durante a renderização de quadros (por exemplo, viewports diferentes para o mundo 3D e HUD). Nesse caso, a origem do On-Screen Display segue um dos cantos da última viewport definida durante a renderização de quadros, que pode estar localizada em uma posição indesejada. As opções relacionadas à substituição do espaço de coordenadas do On-Screen Display podem ser usadas para restaurar a posição de origem esperada em tais aplicativos. Este botão seleciona a viewport de renderização como o espaço de coordenadas para o On-Screen Display.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Espaço de coordenadas de exibição na tela: Framebuffer**  
Por padrão, o espaço de coordenadas do On-Screen Display corresponde ao espaço de coordenadas da viewport de renderização, ou seja, a última área retangular para a qual o aplicativo estava renderizando. No entanto, certos aplicativos (por exemplo, StarCraft II: Wings of Liberty) podem usar várias viewports durante a renderização de quadros (por exemplo, viewports diferentes para o mundo 3D e HUD). Nesse caso, a origem do On-Screen Display segue um dos cantos da última viewport definida durante a renderização de quadros, que pode estar localizada em uma posição indesejada. As opções relacionadas à substituição do espaço de coordenadas do On-Screen Display podem ser usadas para restaurar a posição de origem esperada em tais aplicativos. Este botão seleciona todo o framebuffer como o espaço de coordenadas para o On-Screen Display.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Habilitar sombra de exibição na tela**  
Habilita a renderização de sombras no On-Screen Display. A renderização de sombras pode melhorar a legibilidade do On-Screen Display em alguns aplicativos, evitando que o texto se mescle com cores sólidas da tela. Observe que a renderização de sombras aumenta o impacto no desempenho causado pela renderização do On-Screen Display em modos vetoriais, portanto, habilite-a somente quando necessário.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Habilitar preenchimento de exibição na tela**  
Habilita o preenchimento da área subjacente do On-Screen Display com uma cor sólida ou transparente. A cor de preenchimento e o nível de transparência podem ser ajustados na paleta On-Screen Display. Preencher a área subjacente pode melhorar a legibilidade do On-Screen Display em alguns aplicativos, evitando que o texto se mescle com cores sólidas da tela.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Paleta de exibição na tela: cor base**  
Exibe a cor base para On-Screen Display e permite que você a redefina. Você também pode ajustar o nível de transparência da cor base para os modos de renderização On-Screen Display 3D vetorial e 3D raster.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Paleta de exibição na tela: Cor da sombra**  
Exibe a cor da sombra para On-Screen Display e permite que você a redefina para modos de renderização On-Screen Display de vetor. Você também pode ajustar o nível de transparência da cor da sombra para o modo de renderização On-Screen Display de vetor 3D. Observe que a renderização de sombra aumenta o impacto no desempenho causado pela renderização On-Screen Display em modos de vetor, então habilite-a somente quando necessário.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Paleta de exibição na tela: cor de preenchimento**  
Exibe a cor de preenchimento para On-Screen Display e permite que você a redefina. Você também pode ajustar o nível de transparência da cor de preenchimento para os modos de renderização On-Screen Display 3D vetorial e 3D raster.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Zoom de exibição na tela**  
Ajusta a taxa de zoom do On-Screen Display. Use a janela de pré-visualização do On-Screen Display para controle visual da aparência do On-Screen Display ao aplicar zoom.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Mostrar estatísticas próprias**  
O objetivo principal do RivaTuner Statistics Server é coletar estatísticas de taxa de quadros para todos os aplicativos 3D em execução no sistema e fornecer esses dados para aplicativos clientes, como RivaTuner, HIS iTurbo, EVGA Precision ou MSI Afterburner. Ele também fornece serviços adicionais, como On-Screen Display, suporte para captura de tela ou detecção 3D, para os clientes. No entanto, você também pode usar o RivaTuner Statistics Server como uma solução autônoma de monitoramento de taxa de quadros. Habilite esta opção para permitir que o RivaTuner Statistics Server mostre suas próprias estatísticas de taxa de quadros no On-Screen Display sem executar nenhum aplicativo cliente adicional. Quando os aplicativos clientes estão usando o mecanismo de captura de vídeo do RivaTuner Statistics Server, esta opção também controla a exibição de estatísticas adicionais relacionadas à captura de vídeo. Habilite-o para exibir estatísticas de tempo, tamanho, taxa de compressão por quadro e tempo de compressão do arquivo de vídeo ao lado do indicador de captura de vídeo.  
*Dicas:*  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

---

**Visualização na tela**  
Exibe a pré-visualização do On-Screen Display. Observe que o tamanho e a posição da pré-visualização são precisos apenas para modos de exibição que correspondem ao seu modo de exibição atual e são relativos ao canto de origem.  
*Dicas:*  
- Você pode destacar e definir uma posição e tamanho personalizados para a janela de pré-visualização clicando duas vezes na área da janela de pré-visualização. Isso pode simplificar o processo de ajuste visual da posição do On-Screen Display.  
- Você pode clicar com o botão direito do mouse nesta janela e selecionar o comando *Capture Screenshot* no menu de contexto para capturar uma captura de tela do aplicativo 3D em execução no momento e usá-la como imagem de fundo para esta janela. Isso pode simplificar o processo de ajuste visual da posição On-Screen Display. O fundo padrão pode ser selecionado com o comando *Clear* no menu de contexto.  
- Os sistemas anti-cheat de alguns jogos podem tratar o gancho de código do jogo, necessário para detecção de aplicativos e renderização do On-Screen Display, como um possível cheat e bloquear a conexão com servidores multijogador. Para solucionar esses problemas, tente adicionar um perfil para esse jogo e desabilitar o suporte ao On-Screen Display ou, se isso não ajudar, tente diminuir o nível de detecção do aplicativo.  
- Você pode desabilitar as dicas de ferramentas da interface do usuário por meio da guia *Interface do usuário* nas propriedades avançadas.

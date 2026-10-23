# Prompt para o Lovable — Youcast Channel in a Box

Implemente neste projeto um vídeo comercial em motion design, seguindo o roteiro abaixo.

## Entrega obrigatória

- MP4, Full HD 1920 × 1080, horizontal 16:9.
- Duração exata: 30 segundos, 30 fps (900 frames).
- **Vídeo completamente sem áudio: sem locução, trilha, efeitos sonoros ou faixa de áudio no MP4.**
- Toda a mensagem deve ser compreendida visualmente.
- Prévia com controles de reprodução, pausa, reinício e navegação no tempo.
- Implementar exportação real de MP4 quando o ambiente suportar. Não criar botão fictício, download de arquivo vazio ou exportação WebM apresentada como MP4.
- Se o ambiente não renderizar MP4, entregar composição e instruções reproduzíveis de renderização; explicar a limitação na interface.

## Direção criativa

Produzir um filme de produto com cinco cenas e elementos animados independentes.
Não reutilizar os três posts como slides, nem colocar imagens completas lado a lado com textos repetidos. As artes são referências de identidade.
Usar motion graphics, grade de programação, dispositivos e fluxo de distribuição para explicar o produto.
Identidade: preto/grafite, branco e amarelo Youcast (referência #F3D34A; priorizar arquivos oficiais).
Tipografia forte, títulos curtos, contraste alto, margem de segurança de 96 px nas laterais e 72 px no topo/rodapé.
Usar o logotipo oficial como arquivo, sem redesenhá-lo ou substituí-lo por texto.
Animações com propósito: entradas escalonadas, deslocamentos suaves, máscaras e mudanças de enquadramento.
Evitar excesso de efeitos, zoom contínuo sobre posts, interfaces fictícias apresentadas como capturas reais e textos pequenos.
Fotografias estáticas podem ser usadas como apoio, mas não como substituto de todas as cenas animadas.
Não usar marcas de anunciantes, serviços de streaming ou canais de terceiros sem arquivos autorizados.

## Roteiro com tempos fechados

### Cena 1 — Conteúdo | 00:00–00:05 | frames 0–149
Texto: **SEU CONTEÚDO PODE IR ALÉM.**
Visual: quadros independentes de esporte, entretenimento e jornalismo entram em sequência e se organizam como acervo.
Movimento: composição com profundidade, recortes e destaque amarelo em “IR ALÉM”.
Usar vídeos reais se disponíveis; caso contrário, animar os quadros e seus elementos de forma conceitual.
Reservar pelo menos os últimos 2 segundos para leitura do título.

### Cena 2 — Canal | 00:05–00:12 | frames 150–359
Texto principal: **UM CANAL LINEAR NA NUVEM.**
Apoios sequenciais: **AO VIVO + VOD** e **PROGRAMAÇÃO 24/7**.
Visual: os quadros se transformam em blocos de uma grade. Um marcador percorre a linha do tempo e o conteúdo selecionado aparece em um monitor.
Animar a alternância entre VOD e AO VIVO. O selo deve acompanhar o bloco ativo.
A grade é ilustração conceitual, não uma captura da interface real.
Manter o título por pelo menos 4 segundos; apoios por pelo menos 2 segundos cada.

### Cena 3 — Distribuição | 00:12–00:19 | frames 360–569
Texto principal: **UM CANAL. MÚLTIPLOS DESTINOS.**
Rótulos: **OTT**, **FAST**, **OPERADORAS**.
Visual: o monitor se conecta a TV, tablet e celular por linhas amarelas. O mesmo conteúdo aparece nas telas.
Dispositivos e conexões entram em sequência, com movimento suave e profundidade.
Distribuição é uma possibilidade técnica; não sugerir contratação ou presença garantida em plataformas específicas.
Manter o título por pelo menos 4 segundos.

### Cena 4 — Monetização | 00:19–00:25 | frames 570–749
Texto principal: **NOVAS OPORTUNIDADES DE RECEITA.**
Apoio: **PUBLICIDADE COM SSAI INTEGRADO**.
Visual: aproximar uma tela. Um bloco amarelo “PUBLICIDADE” entra na programação; exibir um anúncio fictício sem marca e retornar ao conteúdo.
A animação deve explicar inserção dinâmica de publicidade; não exibir métricas de faturamento nem promessas de retorno.
Manter o título por pelo menos 4 segundos e o apoio por pelo menos 3 segundos.

### Cena 5 — Encerramento | 00:25–00:30 | frames 750–899
Elementos:
- Logotipo oficial YOUCAST.
- **CHANNEL IN A BOX**
- **SEU CANAL. NOVAS POSSIBILIDADES.**
- **FALE COM A YOUCAST**
- **youcast.tv.br**
- Assinatura discreta: **Powered by Uplynk**.
As conexões amarelas convergem para a marca.
Concluir entradas até 00:27 e manter o quadro final estável de 00:27 a 00:30.
Se houver fade final, preservar a leitura até pelo menos 00:29,5.

## Implementação

Inspecionar a estrutura existente antes de escolher a implementação. Se ainda não houver aplicação, criar a estrutura necessária.
Uma composição React/Remotion com timeline determinística é uma opção; usar tecnologia compatível com o ambiente.
Separar cenas e componentes reutilizáveis: marca, título, bloco da grade, dispositivo e conexão.
Usar timeline baseada em frames, com semente fixa para qualquer variação visual.
Disponibilizar textos e referências de mídia em configuração editável.
Todas as durações de transição fazem parte dos intervalos das cenas, sem aumentar a duração total.
Não solicitar microfone, não gerar arquivos de áudio e não usar autoplay com som.
Não inserir músicas ou narração “opcionais” na versão entregue.

## Assets e recursos

Os anexos da conversa não são automaticamente arquivos deste repositório.
Usar arquivos oficiais de marca e mídia fornecidos no Lovable ou presentes no projeto.
Se o logotipo ou mídia estiverem ausentes, sinalizar os itens necessários e oferecer campos para substituição.
Usar representações conceituais para grade e dispositivos enquanto não houver capturas reais.
Não apresentar placeholders como materiais oficiais aprovados.

## Validação

1. Exatamente 900 frames / 30 segundos.
2. 1920 × 1080, pixels quadrados, 16:9, 30 fps.
3. MP4 com vídeo H.264 e pixel format yuv420p para compatibilidade.
4. Nenhuma faixa de áudio.
5. Sem cortes de texto, sobreposições ou deformação de marca e dispositivos.
6. Conferir o início, as quatro transições e o encerramento.
7. Verificar a reprodução do MP4 exportado, não apenas a prévia.
8. Toda a narrativa deve funcionar sem som.

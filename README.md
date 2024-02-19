# PROJETO: Utilizando VISION para Reconhecimento Facial e transformação de Imagens em Dados na linguagem computacional.

Olá! Me chamo Isac Freitas, e este é meu projeto trabalhando com a ferramenta Vision da Microsoft Azure AI, para Reconhecimento Facial e transformação de Imagens em Dados.

Bom, para o projeto, foram dadas as instruções no curso de Microsoft Azure Ai Fundamentals pela plataforma DIO, com todos os dados para os alunos entregarem a atividade.

Foram compartilhados três links (documentações de apoio):

1- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html



2- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html



3- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html


Lembrando que antes de tudo, você tem que ir no portal da Azure e criar um recurso de Video Indexer de IA, do Próprio Azure. Se você não tiver um recurso de Indexer de IA, vai ter que fazer isso antes do processo, se não, não vai conseguir utilizar o Azure AI Vision.

--------------------------

### 1- Pré-projeto.

--------------------------

Entramos em https://www.portal.azure.com e vamos em "Criar um recurso".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/22fd155a-e29b-49c3-ab68-2b5411736fca" width="900px" />
</div>

Na caixinha "Serviços de pesquisa e marketplace", digitamos "Azure AI services" e Enter.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/f03565d1-0a50-41cf-b317-c56169bc1a49" width="900px" />
</div>

*DICA: se aparecer uma caixa acima de sua pesquisa que diz "Obtenha sugestões geradas por IA para sua pesquisa", clique em "Exibir sugestões" para que os resultados sejam melhores .
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/183bfdfa-5a79-4106-8510-2fd15efe925d" width="900px" />
</div>

Agora, com as sugestões por IA habilitadas, 
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/3d5017ae-d41b-4310-a9cb-1f97900bd415" width="900px" />
</div>

descemos até a parte de "Produtos sugeridos", e clicamos sobre "Azure AI Services".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/efbaf330-76e9-4cc2-a35d-ffd3c1632782" width="900px" />
</div>

*DICA: caso não apareça de primeira a opção de "Azure AI Services", é só descer mais ou pouco ou pesquisar "Serviços Cognitivos", porém nesta segunda alternativa, certifique-se que a licenciatura deste produto está como "Microsoft | Zure Service".



Aqui, escolhemos nosso plano, e clicamos em Criar.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/ee157b05-7f65-4165-b581-ad728715e621" width="900px" />
</div>

Aqui, você cria ou seleciona um Grupo de recursos para ser usado neste projeto.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/89c7f8ab-7c04-44fe-808e-e1a9c6b94739" width="900px" />
</div>

Agora, descendo mais um pouco na página, você define a região do servidor, o nome do Projeto e o tipo de preço (recomendo que ponha em Standard S0). Marca a caixinha que diz que você entende os termos de uso
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/dd186314-34fe-4a2f-bc30-9f97a6ce8ead" width="900px" />
</div>

Por último, clique em "Examinar + criar", revise se escreveu e selecionou tudo corretamente, e crie. 
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/86b19ef4-d2c1-49c1-862b-b9dbf8fa3ed5" width="900px" />
</div>

Agora espere a implantação terminar, e ao terminar, clique em ir para o recurso (você não vai precisar fazer nada lá).
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/0b793a3b-94e1-44a5-b55a-af17f9f201ec" width="900px" />
</div>

--------------------------

### 2- Reconhecimento facial.

--------------------------

Bom, você vai entrar no portal Vision do Microsoft Azure (https://portal.vision.cognitive.azure.com/).
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/151ad437-83c8-4f11-8410-c6502d5ed3ca" width="900px" />
</div>

Agora, clique na aba Face.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/f662f48a-6ba7-4e91-a856-0cf5feeb7492" width="900px" />
</div>

Nessa parte, aparece a opção "Detect faces in an image". Então cliquei em "Try it out" para prosseguirmos.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/5566469b-ac1c-4410-b401-e6400f11abf3" width="900px" />
</div>

Aqui, marco essa caixa, permitindo uso de imagem, e aceitar os termos.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/09b40029-5f6d-4bdc-9343-80291c53e851" width="900px" />
</div>

Agora seleciono a imagem em "Browse for a file" a imagem que desejo usar para nosso teste.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/190e5847-a992-4b27-92b4-ec350864c4de" width="900px" />
</div>

Descendo mais um pouco a página, podemos ver o resultado do nosso teste.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/bf7ec831-fb4c-43fa-93d6-289816bfd1ae" width="900px" />
</div>

A ferramenta seleciona todo o rosto de pessoas da imagem que você selecionar. 
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/00812973-9c67-4edf-842a-5f8dd5b50e7a" width="900px" />
</div>

--------------------------

### 3- Reconhecimento e descrição de imagens.

--------------------------

Volte para a pagina inicial do Vision e entre na aba "Image Analysis".
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/0961a855-30f7-494e-927c-9446af05679a" width="900px" />
</div>

Desça a página até encontrar a opção "Add captions to images", e clique em Try It Out.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/29b50d5e-dc97-41a2-a871-040a8d50e2df" width="900px" />
</div>

Aqui, vou selecionar a imagem de paisagem que vamos analisar.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/53b03b9e-08df-4612-a5cc-3a1081ec4684" width="900px" />
</div>

Após o upload da imagem:
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/e2de4ad5-e577-43fe-bdac-6718f6fb0e2f" width="900px" />
</div>

A descrição, no caso, foi feita em inglês. Mas basicamente, a inteligência artificial descreveu como "Corpo de água com pessoas nadando".

--------------------------

### 4- Reconhecimento de texto em imagens.

--------------------------

De volta a página inicial, vamos na aba "Optical Character Recognition" (ou Reconhecimento optico de caractéres), e vamos na sua única opção e clicamos em Try It Out.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/6cb682e5-bf51-4aa0-ae1f-a9d4e5ee36e8" width="900px" />
</div>

Aqui, vou carregar a imagem que separei para o nosso teste.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/12ac9e68-a2cc-4bd8-9110-7fb10bee54b1" width="900px" />
</div>

Descendo mais um pouco a página, podemos ver o resultado do nosso teste.
<div align="center">
<img src="https://github.com/IsacFreitaas/Projeto-Microsoft-Azure-AI-Vision/assets/65254733/06fbe697-0d48-4896-a9f4-08ae0be99e1a" width="900px" />
</div>

Aqui está nosso resultado. A máquina reconheceu todos o caractéres que formam palavras, porém não reconheceu a palavra "Day".

Mas não tem problema! Ao longo do tempo, a tendência é que a inteligência artificial vá se auto-aprimorando, e que vá ficando cada vez mais próxima de seu potencial.

Obrigado por me acompanhar nestes testes até aqui!

--------------------------

Então é isso.

# Este foi o meu primeiro projeto em Vision da Microsoft Azure ML, em meus estudos em Ciência de Dados.

Obrigado pela atenção!

**Qualquer dúvida sobre o projeto, ou caso precise de auxílio, fico a disposição. Entre em contato comigo por meio de minhas redes sociais (listadas abaixo ou em meu perfil).

--------------------------

Sobre mim:
# Isac Freitas
Atualmente estudante de Ciência de Dados e Inteligência Artificial.

### Me encontre:

Insta: @isac.sfreitas



Twitter: @isaczeitgeist

# Projeto-Microsoft-Azure-AI-Vision

Reconhecimento Facial e transformação de Imagens em Dados no Microsoft Azure ML

Olá! Me chamo Isac Freitas, e este é meu projeto trabalhando com a ferramenta Vision da Microsoft Azure ML, para Reconhecimento Facial e transformação de Imagens em Dados.

Bom, para o projeto, foram dadas as instruções no curso de Microsoft Azure Ai Fundamentals pela plataforma DIO, com todos os dados para os alunos entregarem a atividade.

Foram compartilhados três links (documentações de apoio):

1- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/04-face.html



2- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/05-ocr.html



3- https://microsoftlearning.github.io/mslearn-ai-fundamentals/Instructions/Labs/03-image-analysis.html


Lembrando que antes de tudo, você tem que ir no portal da azure e criar um recurso de Video Indexer de IA, do Próprio Azure. Se você não tiver um recurso de Indexer de IA, vai ter que fazer isso antes do processo, se não, não vai conseguir utilizar o Azure AI Vision.

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

*DICA: se aparecer uma caixa acima de sua pesquisa que diz "Obtenha sugestões geradas por IA para sua pesquisa", clique em "Exibir sugestões para que os resultados sejam melhores.
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

Agora, clique na aba Face.

Nessa parte, aparece a opção "Detect faces in an image". Então cliquei em "Try it out" para prosseguirmos.

Aqui, marco essa caixa, permitindo uso de imagem, e aceitar os termos.

Agora seleciono a imagem em "Browse for a file" a imagem que desejo usar para nosso teste.

Descendo mais um pouco a página, podemos ver o resultado do nosso teste.

A ferramenta seleciona todo o rosto de pessoas da imagem que você selecionar. 

parte 2- agora vamos testar a ferramenta de reconhecimento e descrição de paisagens.

Volte para a pagina inicial do Vision e entre na aba "Image Analysis".

Desça a página até encontrar a opção "Add captions to images", e clique em Try It Out.

Aqui, vou selecionar a imagem de paisagem que vamos analisar.

A descrição, no caso, foi feita em inglês. Mas basicamente, a inteligência artificial descreveu como "Corpo de água com pessoas nadando".

parte 3- reconhecimento de texto em imagem.

De volta a página inicial, vamos na aba "Optical Character Recognition" (ou Reconhecimento optico de caractéres), e vamos na sua única opção e clicamos em Try It Out.

Aqui, vou carregar a imagem que separei para o nosso teste.

descendo mais um pouco a página, podemos ver o resultado do nosso teste.

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

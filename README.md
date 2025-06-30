# DIO-Language-Speech
Documentação a respeito da utilização das ferramentas de voz e linguagem do Microsoft Azure, nominalmente, Language Studio e Speech Studio.

## Descrição do projeto

Neste documento serão abordados alguns aspectos acerca da criação de ferramentas de conversão e reconhecimento de voz em texto disponíveis nas plataformas [Azure Language Studio](https://language.cognitive.azure.com/home) e [Azure Speech Studio](https://speech.microsoft.com/portal) e de sua utilização. Será um guia introdutório, a documentação completa das plataformas pode ser acessada nos links: [Azure Speech Studio](https://learn.microsoft.com/pt-br/azure/ai-services/speech-service/) e [Azure Language Studio](https://learn.microsoft.com/pt-br/azure/ai-services/language-service/).

### Implantação
#### Portal Azure
Primeiramente, é necessário implantar um novo recurso no [Portal Azure](https://portal.azure.com/). Para tal, siga os passos a seguir:
  
1. No menu do topo da página, à esquerda, clique em **Criar recurso**, indicado com um **+**.  
2. Pesquise por **Language** e selecione **Serviço de Linguagem**.  
3. Selecione se deseja incluir algum serviço adicional, como Custom question answering (respostas de perguntas personalizadas) e Custom text classification, Custom named entity recognition, Custom sentiment analysis & Custom Text Analytics for health (Classificação de texto personalizada, reconhecimento de entidade com nome personalizado, análise de sentimento personalizada e análise de texto personalizada para saúde) e continue para a criação do recurso.
4. Preencha o formulário, como mostrado na [Figura 1](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L1.jpg):  
   - Subscription: escolha sua assinatura.
   - Resource group: selecione um grupo existente ou crie um novo.  
   - Nome: algo como `my-language-service`.  
   - Região: escolha perto de você (ex.: Brazil South).  
   - Tier: comece com **F0 (gratuito)** para testes.  
5. Clique em **Revisar + criar** e depois em **Criar** na tela de revisão do novo recurso.

O próximo passo natural é acessar o recurso no Portal Azure, [Figura 2](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L2.jpg), o que nos redireciona diretamente para a página do [Azure Language Studio](https://language.cognitive.azure.com/home), mas com já com a janela para criação de um novo recurso aberta, [Figura 3](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L3.jpg)

### Language Studio

Como mostrado na Figura 3, há a possibiliadde de escolher-se o tipo de serviço desejado, entre serviços cognitivos, linguagem e tradutor. Escolha o mais adequado. Vou prosseguir utilizando a opção linguagem, usando a minha assinatura e as configurações escolhidas durante a criação do recurso no Portal Azure.

Uma vez criado o recurso de linguagem, existem diversas opções de tarefas a serem feitas, com várias opções dentro de cada menu, mostradas nas figuras da descrição, como [extrair informações](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L4.jpg), [classificar texto](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L5.jpg), [entender questões e linguagem conversacional](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L6.jpg), [sumarizar texto](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L7.jpg) e [traduzir texto ](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L8.jpg). Escolha a opção desejada e divirta-se! Há uma infinidade de funções nessa plataforma.

### Speech Studio

A interface do Speech Studio é bastante mais direta, logo na homepage, existem as opções de [Recursos de fala por situação](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L9.jpg), [Conversão de fala em texto](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L10.jpg), [Conversão de texto em fala](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L11.jpg) e [Assistente de voz](https://github.com/msccobra/DIO-Language-Speech/blob/Images/L12.jpg). Basta apenas clicar na opção desejada e será direcionado.

Alguns dos serviços, como o de conversão de fala em texto permitem uma demonstração, onde você fala no microfone e sua voz é convertida em texto, ou pode ser usado um arquivo de áudio pequeno, ate 1 minuto, antes de se configurar a criação de um novo recurso. Para ulguns outros serviços, essa demonstração não estará disponível.

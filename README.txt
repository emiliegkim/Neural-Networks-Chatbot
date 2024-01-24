README

Autoras: Emilie Ga Eun Kim e Mariana Luísa Gonçalves da Silva

-- AIML Chatbot 

	Este código implementa um chatbot utilizando AIML (Artificial Intelligence Markup Language), uma linguagem de marcação para a criação de agentes virtuais. O chatbot é especializado em Redes Neurais Artificiais e interage com o usuário através de uma interface de linha de comando.
	
	O arquivo AIML deste Chatbot 'base.aiml' contém 13 perguntas sobre Redes Neurais Artificias com respostas que partem de fontes confiáveis, ao final de cada resposta foi colocada a devida referência.

-- Pré-requisitos
	Certifique-se de que o pacote python-aiml está instalado. Caso contrário, instale utilizando o seguinte comando:

!pip install python-aiml

-- Configuração do Google Colab

	1. Monte o Google Drive no ambiente Colab usando:
	
	from google.colab import drive
	drive.mount('/content/drive')

	2. Altere o diretório de trabalho para o local onde o arquivo AIML está armazenado, substituindo o caminho de acordo com seu diretório específico:

	%cd "/content/drive/MyDrive/UFCSPA/4º Semestre/IA/trabalho final IA"
	
-- Carregamento da Base de Conhecimento AIML

	1. Importe o módulo AIML:
	
	import aiml
	
	AIML (Artificial Intelligence Markup Language) é uma linguagem de marcação específica para a criação de chatbots e sistemas de processamento de linguagem natural (PLN). Desenvolvida inicialmente por Richard Wallace nos anos 1990, AIML foi projetada para ser uma linguagem padrão para a criação de agentes de conversação ou chatbots, facilitando a codificação de padrões de diálogo e respostas associadas.
	
	2. Crie o kernel AIML:
	
	kernel = aiml.Kernel()
	
	No AIML (Artificial Intelligence Markup Language), o "kernel" refere-se à instância central que interpreta as instruções AIML e gerencia a interação do chatbot. O kernel AIML é uma espécie de "cérebro" do chatbot AIML, responsável por interpretar as entradas do usuário, procurar correspondências nos padrões AIML e gerar as respostas correspondentes.

	3. Defina o caminho do arquivo AIML que contém a base de conhecimento. Modifique o caminho de acordo com a localização do seu arquivo:

	base_conhecimento_aiml_file = '/content/drive/MyDrive/UFCSPA/4º Semestre/IA/trabalho final IA/base.aiml'

	4. Carregue a base de conhecimento AIML utilizando o método learn:

	kernel.learn(base_conhecimento_aiml_file)

-- Diálogo com o Chatbot

	1. Inicie o diálogo com o chatbot:
	
	print("Chatbot Especialista em Redes Neurais Artificiais:")
	print("Olá! Como posso ajudar você hoje? (Digite 'sair' para encerrar)")

2. O código entra em um loop infinito, aguardando a entrada do usuário.

3. O usuário pode digitar mensagens. Se a entrada for 'sair', o chatbot exibirá uma mensagem de despedida e encerra o loop.

4. Caso contrário, o kernel AIML processará a entrada do usuário e gerará uma resposta. A resposta é exibida no formato "Chatbot: [resposta]".

5. O ciclo de interação continua até que o usuário escolha sair digitando 'sair'.

Observação: Certifique-se de ajustar os caminhos dos arquivos de AIML de acordo com a localização real dos seus arquivos. O código está configurado para funcionar no ambiente do Google Colab com o Google Drive.




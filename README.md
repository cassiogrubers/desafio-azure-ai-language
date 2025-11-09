# Desafio Prático: Análise de Fala e Linguagem com Azure AI

Este repositório documenta a execução do desafio prático de utilização dos serviços de Speech (Fala) e Language (Linguagem) do Microsoft Azure. O objetivo foi explorar as funcionalidades do **Azure Speech Studio** e **Azure Language Studio** para realizar análises de voz e texto, e documentar os *insights* adquiridos durante o processo.

## 🛠️ Ferramentas Utilizadas

* **Microsoft Azure Portal:** Para criação e gerenciamento dos recursos cognitivos.
* **Azure Speech Studio:** Utilizado para explorar funcionalidades de conversão de voz em texto (Speech-to-Text) e texto em voz (Text-to-Speech).
* **Azure Language Studio:** Utilizado para explorar funcionalidades de Processamento de Linguagem Natural (NLP), como análise de sentimento e reconhecimento de entidades.
* **GitHub:** Para versionamento e documentação deste projeto.

---

## 🚀 Passo a Passo da Execução

Abaixo estão os passos seguidos para a conclusão do laboratório, desde a configuração no portal Azure até a análise nos estúdios.

### 1. Configuração do Ambiente no Azure

1.  Acesso ao [Portal Azure](https://portal.azure.com/).
2.  Criação de um novo Recurso de **Serviços Cognitivos** (ou um recurso de **Fala** e **Linguagem** separadamente, dependendo dos objetivos do laboratório).
3.  Definição do grupo de recursos, região (ex: *East US*) e o tipo de preço (ex: *Free F0*).
4.  Após a criação, as chaves de API e o *endpoint* do recurso foram disponibilizados para autenticação nos estúdios.
<img width="1913" height="669" alt="01-azure-portal-recurso" src="https://github.com/user-attachments/assets/4e6cb9ce-3f65-41b5-a520-b9abae181b32" />

   

### 2. Explorando o Azure Speech Studio

Utilizei o Speech Studio para testar a funcionalidade de **Speech-to-Text (STT) em tempo real**.

1.  Acessei o [Speech Studio](https://speech.microsoft.com/) e autentiquei com o recurso de Fala criado.
2.  Naveguei até a funcionalidade "Reconhecimento de fala em tempo real".
3.  Utilizei o microfone para falar uma frase de teste (ex: "Olá, este é um teste para o serviço de fala do Azure.") ou carreguei um arquivo de áudio.
4.  Analisei a transcrição gerada automaticamente pela ferramenta.

* *Resultado da Transcrição:*
<img width="1905" height="836" alt="02-speech-studio-transcricao" src="https://github.com/user-attachments/assets/daf451fa-7e87-4298-aaad-e3edcc8f9952" />


### 3. Explorando o Azure Language Studio

No Language Studio, o foco foi em **Análise de Sentimento** e **Reconhecimento de Entidades Nomeadas (NER)**.

1.  Acessei o [Language Studio](https://language.cognitive.azure.com/) e selecionei o recurso de Linguagem.
2.  Naveguei até a funcionalidade "Analisar sentimento e extrair opiniões".
3.  Inseri um texto de exemplo (ex: "A comida estava deliciosa e o ambiente era muito agradável, mas o atendimento foi péssimo.").
4.  Analisei o resultado, que identificou o sentimento geral (Misto/Neutro) e os sentimentos específicos por alvo ("comida" = positivo, "atendimento" = negativo).

* *Resultado da Análise de Sentimento:*
<img width="1898" height="967" alt="03-language-studio-sentimento" src="https://github.com/user-attachments/assets/5a56cc71-bf46-4806-b1b3-c888912014f3" />



5.  Em seguida, testei a "Detecção de idioma".
6.  Inseri um texto (ex: "La qualité de ce produit est incroyable." ou "This is a wonderful test.").
7.  Analisei o resultado, que identificou corretamente o idioma (ex: Francês, Inglês) e a pontuação de confiança (ex: 1.0).

* *Resultado da Detecção de Idioma:*
<img width="1907" height="882" alt="02-detecção-do-idioma" src="https://github.com/user-attachments/assets/a9267823-6047-4050-a3d0-63c81eeafa09" />



---

## 🧠 Resultados e Insights Adquiridos

Esta seção documenta os principais aprendizados e observações durante o laboratório.

* Facilidade de Uso (Interface Gráfica):  "Achei a interface dos estúdios muito intuitiva. Mesmo sem conhecimento prévio de código, foi possível testar funcionalidades complexas de IA rapidamente.
* **Precisão dos Modelos:** "A precisão da transcrição de fala foi impressionante, reconhecendo corretamente termos técnicos. A análise de sentimento foi capaz de capturar a nuance de uma frase com sentimentos mistos, o que é um desafio comum.
* **Descoberta Chave:** "O mais interessante foi a capacidade da Análise de Sentimento de não apenas dar uma nota geral, mas de identificar o sentimento associado a entidades específicas (mineração de opinião). Isso tem um valor comercial imenso para análise de feedback.
* **Desafios Encontrados:**"Tive uma breve confusão inicial para entender qual tipo de recurso criar no Azure (Recurso único de Serviços Cognitivos vs. recursos separados de Fala/Linguagem) para habilitar todas as funcionalidades dos estúdios.

---

## 🏁 Conclusão

Este laboratório foi uma excelente oportunidade para aplicar na prática os conceitos das vídeo-aulas. A capacidade de testar modelos de IA de ponta diretamente no navegador, sem escrever código, desmistifica o uso dessas tecnologias. A documentação do processo no GitHub serviu para solidificar o aprendizado e criar um material de consulta valioso. As ferramentas de IA do Azure são poderosas e surpreendentemente acessíveis.

# Projeto SICOMUV

Este repositório contém o projeto SICOMUV, um assistente de comunicação e tradução desenvolvido para facilitar a interação com diversos idiomas através de processamento de imagem, reconhecimento de texto e tradução automática.

## Estrutura do Repositório

- **H5/**
  - `H5.h5`: Modelo treinado usado para processamento de imagem e reconhecimento de padrões.

- **.gitattributes**: Arquivo de configuração para atributos específicos do Git, garantindo consistência ao lidar com diferentes sistemas operacionais.

- **Apresentação.py**: Script principal que implementa as funcionalidades do SICOMUV, incluindo reconhecimento de voz, tradução de texto e interação com o usuário.

- **Apresentação.txt**: Arquivo de texto complementar que pode conter informações adicionais ou logs gerados pelo script.

- **README.md**: Este arquivo, que fornece uma visão geral do projeto, suas funcionalidades e instruções de uso.

- **requirements.txt**: Lista de dependências Python necessárias para executar o projeto. Inclui bibliotecas como OpenCV, pytesseract, Keras, entre outras.

## Funcionalidades do `Apresentação.py`

O script `Apresentação.py` é o núcleo do projeto SICOMUV e oferece as seguintes funcionalidades:

- **Reconhecimento de Voz**: Captura comandos de voz do usuário para controlar o fluxo do programa, como capturar imagens ou encerrar o programa.

- **Tradução Automática**: Traduz texto extraído de imagens para um idioma escolhido pelo usuário através de comandos de voz.

- **Processamento de Imagem**: Utiliza OpenCV para capturar e processar imagens, convertendo-as em texto utilizável.

- **Interação por Voz**: Usa o `pyttsx3` para sintetizar voz, fornecendo feedback auditivo ao usuário durante a operação.

- **Configuração de Idiomas**: Suporta uma ampla gama de idiomas para tradução, configuráveis via comandos de voz.

### Detalhes Técnicos

- **Configuração do Tesseract**: O script está configurado para usar o Tesseract OCR instalado no diretório `C:\Program Files\Tesseract-OCR\`.

- **Modelo de Machine Learning**: Carrega um modelo Keras a partir do arquivo `H5.h5` para auxiliar no processamento de imagens.

- **Paralelismo**: Utiliza `ThreadPoolExecutor` para executar tarefas de reconhecimento de voz e captura de imagem simultaneamente.

## Como Executar

1. **Instalar Dependências**: Execute `pip install -r requirements.txt` para instalar todas as bibliotecas necessárias.

2. **Configurar Tesseract**: Certifique-se de que o Tesseract OCR está instalado no caminho especificado no script.

3. **Executar o Script**: Inicie o programa executando `python Apresentação.py` no terminal.

4. **Interagir com o Assistente**: Use comandos de voz para capturar imagens ou solicitar traduções.

## Contribuição

Contribuições são bem-vindas! Sinta-se à vontade para abrir issues ou enviar pull requests para melhorias.

## Licença

Este projeto está licenciado sob a MIT License - veja o arquivo [LICENSE](LICENSE) para mais detalhes.
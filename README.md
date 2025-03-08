# Tesouro Direto Monitor

## 📋 Descrição

O **Tesouro Direto Monitor** é um script Python desenvolvido para automatizar a coleta de dados do Tesouro Direto, processar as informações e enviar atualizações em tempo real via Telegram. Ele utiliza Selenium para extração de dados da web e organiza os títulos de acordo com os melhores retornos.

## 🚀 Funcionalidades

- Coleta automática de dados do Tesouro Direto.
- Processamento e classificação de títulos públicos (IPCA+, Prefixado, etc.).
- Formatação de mensagens personalizadas para Telegram.
- Envio automático de atualizações usando um bot do Telegram.

## 🧰 Tecnologias Utilizadas

- **Python 3.13.1**
- **Selenium** para automação de navegador.
- **pylegram** para integração com o Telegram.
- **JSON** para manipulação de dados.

## ⚙️ Instalação

1. Clone o repositório:
   ```bash
   git clone https://github.com/seu-usuario/seu-repositorio.git
   cd seu-repositorio
   ```

2. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

3. Configure o WebDriver do Chrome, garantindo que esteja compatível com a sua versão do navegador.

## 🔑 Configuração

- **Token do Telegram:** Altere o token do bot e o `chat_id` no arquivo `MessageSender` para os seus dados.
- **WebDriver:** Ajuste as configurações do Selenium se necessário (ex: modo headless).

## 🚩 Como Usar

Execute o script principal:

```bash
python main.py
```

O script irá:
- Coletar dados atualizados do Tesouro Direto.
- Processar os títulos para exibir os melhores rendimentos.
- Enviar uma mensagem formatada para o Telegram.

## 🗂️ Estrutura do Projeto

```
.
├── main.py              # Script principal
├── requirements.txt     # Dependências do projeto
├── README.md            # Documentação
└── src/
    ├── chrome_config.py   # Configuração do WebDriver
    ├── data_fetcher.py    # Coleta de dados do Tesouro Direto
    ├── data_processor.py  # Processamento dos dados
    ├── message_formatter.py  # Formatação da mensagem
    └── message_sender.py     # Envio da mensagem via Telegram
```

## ✅ Exemplo de Saída

```
🤖 *Monitoramento #TesouroDireto*

*IPCA+*
• 2029  5.75%  R$1010.00

*Prefixado*
• 2026  10.25%  R$950.00

#investimentos #rendafixa #IPCA
```

## 📄 Licença

Este projeto é privado e protegido por direitos autorais. O uso e a distribuição estão restritos.

## 🤝 Contato

Desenvolvido por [@fcardan](https://www.linkedin.com/in/fcardan/).

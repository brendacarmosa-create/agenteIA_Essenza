# Assistente Essenza | Agente de IA interno

🧑‍💻 **Projeto pessoal (estudo)** · cenário e dados fictícios

🌐 **Converse com a Essenza:** https://brendacarmosa-create.github.io/agenteIA_Essenza/

> Minha primeira agente de IA: orienta a equipe de uma clínica de estética fictícia no sistema de caixa FluxoCerto, com base nos POPs, sem inventar respostas.

## O problema
Em uma clínica, a equipe tem dúvidas no dia a dia sobre como usar o sistema de caixa: cadastrar cliente, lançar pagamento, registrar despesa, fazer devolução e fechar o caixa. Procurar no manual toma tempo e gera erro.

## A solução
A Essenza é uma assistente interna que responde essas dúvidas seguindo os POPs (Procedimentos Operacionais Padrão) e mostra o passo a passo com imagens do sistema. Se a resposta não está no POP, ela não inventa.

## O que ela sabe responder
- Cadastro de cliente
- Lançamento de pagamento por forma (dinheiro, crédito, débito)
- Lançamento de despesa e guarda de comprovantes de fornecedor
- Devolução
- Histórico de pagamentos
- Saldo e conferência do caixa no fim do dia

## Como funciona
1. A pessoa escreve a dúvida na interface (HTML, CSS e JavaScript, publicada no GitHub Pages).
2. A mensagem vai para o fluxo no n8n, que consulta os POPs e chama o Gemini (Google AI Studio). A chave da API do Gemini fica protegida no n8n.
3. A resposta volta para o chat com o passo a passo.

## Tecnologias
n8n · Gemini API · JavaScript · HTML e CSS · GitHub Pages

## Próximos passos
- Criar um back intermediário no Render para guardar a chave do webhook do n8n fora do HTML
- Versionar os POPs no GitHub, para a versão nova substituir a base quando uma regra mudar
- Registrar numa planilha do Google Drive as perguntas que não estão no POP, para ver a frequência e atualizar os POPs

## Autora
**Brenda Carmosa** · [LinkedIn](https://www.linkedin.com/in/brenda-carmosa-30208b361/) · [Portfólio](https://brendacarmosa-create.github.io)

> Aviso: a clínica, o sistema FluxoCerto e todos os dados são fictícios.

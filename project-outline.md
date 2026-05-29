# Projeto Mobile Online - Manager Football

## Objetivo
Criar um jogo de gerenciamento de futebol mobile usando React Native como cliente e um backend online para persistência, autenticação e lógica de partidas.

## Visão geral
- Cliente: React Native (Android/iOS)
- Servidor: API REST ou GraphQL
- Banco de dados: PostgreSQL / MongoDB / Firebase
- Autenticação: email/senha ou OAuth

## Componentes principais
1. Frontend React Native
   - Telas de login/cadastro
   - Dashboard do clube
   - Elenco e escalação
   - Mercado de transferências
   - Treinos e gestão de equipe
   - Liga e agenda de jogos
   - Partida ou resumo de resultado

2. Backend
   - Autenticação e usuários
   - Persistência do estado do clube
   - Lógica de agenda e resultados
   - API para leitura e atualização
   - Rotas para carregar e salvar o jogo

3. Banco de dados
   - Usuários
   - Clubes e times
   - Jogadores e atributos
   - Agenda de partidas
   - Resultados e histórico financeiro

## Roadmap de desenvolvimento
1. Extrair a lógica atual em módulos reutilizáveis
2. Criar o backend básico com endpoints de login e estado do jogo
3. Montar o app React Native com navegação entre telas
4. Implementar sincronização do estado via API
5. Adicionar persistência no servidor
6. Ajustar para online com múltiplos jogadores ou ligas concorrentes

## Considerações importantes
- Não confie no estado guardado no cliente
- Valide todas as entradas no servidor
- Use HTTPS e proteção de sessão
- Mantenha a UI mobile-friendly e otimizada para toque
- Sirva somente os dados necessários ao cliente

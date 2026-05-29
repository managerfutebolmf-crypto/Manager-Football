# Estrutura do Projeto - Manager Football Online

## 1. Estrutura sugerida do repositório

```
manager-football/
├── mobile/
│   ├── App.js
│   ├── package.json
│   ├── src/
│   │   ├── assets/
│   │   ├── components/
│   │   │   ├── ClubCard.js
│   │   │   ├── MatchCard.js
│   │   │   ├── PlayerCard.js
│   │   │   └── StatRow.js
│   │   ├── screens/
│   │   │   ├── LoginScreen.js
│   │   │   ├── RegisterScreen.js
│   │   │   ├── DashboardScreen.js
│   │   │   ├── SquadScreen.js
│   │   │   ├── TrainingScreen.js
│   │   │   ├── MarketScreen.js
│   │   │   ├── LeagueScreen.js
│   │   │   └── MatchScreen.js
│   │   ├── services/
│   │   │   ├── api.js
│   │   │   ├── auth.js
│   │   │   └── game.js
│   │   ├── store/
│   │   │   ├── gameSlice.js
│   │   │   └── userSlice.js
│   │   └── utils/
│   │       ├── format.js
│   │       └── simulation.js
│   └── README.md
├── server/
│   ├── package.json
│   ├── src/
│   │   ├── controllers/
│   │   ├── models/
│   │   ├── routes/
│   │   ├── services/
│   │   └── app.js
│   ├── config/
│   └── README.md
└── README.md
```

## 2. Backend - endpoints principais

- `POST /auth/register`
- `POST /auth/login`
- `GET /game/state`
- `POST /game/save`
- `POST /game/advance-time`
- `GET /game/league`
- `POST /game/match/play`
- `GET /game/market`

## 3. Modelo de dados básico

### Usuário
- id
- email
- senha (hash)
- clube_id

### Clube
- id
- nome
- sigla
- saldo
- moral
- infraestrutura
- elenco
- tática
- agenda
- resultados

### Jogador
- id
- nome
- posição
- atributos
- salário
- contrato
- status de lesão

### Agenda de jogos
- id
- data
- hora
- casa
- fora
- status
- g1
- g2
- resultado

## 4. Telas mínimas do app

- Login / Cadastro
- Dashboard
- Elenco
- Treino
- Mercado
- Liga
- Partida / Resultados

## 5. Como começar

1. Criar o backend com `Node.js + Express` ou `NestJS`
2. Criar o app React Native com `expo init` ou `npx react-native init`
3. Consumir a API do backend no app mobile
4. Armazenar o estado local com Redux, Context ou AsyncStorage
5. Testar fluxo de login, carregar jogo e salvar estado

## 6. Sugestão de prioridade

1. API de autenticação e persistência
2. Regras de jogo e agenda no backend
3. Tela de dashboard e liga no mobile
4. Tela de elenco e mercado
5. Sincronização de partidas e resultados

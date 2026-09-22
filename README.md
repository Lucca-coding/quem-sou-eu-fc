# Quem Sou Eu? FC — BETA 0.1

## Como abrir
Como o jogo carrega `arquivos JSON por modo`, abra a pasta com um servidor local.
Opções rápidas:
- VS Code + extensão Live Server: clique com botão direito em `index.html` > Open with Live Server
- Python: `python3 -m http.server 8080` dentro da pasta e acesse `http://localhost:8080`

## Mecânica
- 3 modos: Europa, Brasileirão e Lendas
- autocomplete: o jogador digita o próprio chute; não há múltipla escolha
- 8 tentativas
- verde = atributo correto
- cinza = incorreto
- setas em idade/ano de nascimento e camisa
- sequência salva em localStorage
- novo jogador aleatório sem repetir imediatamente

## Banco BETA
- Europa: 100 jogadores, 20 por cada uma das 5 grandes ligas
- Lendas: 100 nomes (baseada na ideia de Icons/ÍDOLOS)
- Brasileirão: mix de jogadores atuais e históricos

### Observação de dados
A estrutura aceita `shirt: null`; nesses casos a interface mostra “—”.
Isso evita inventar camisa quando o número atual não está confirmado.
Para Lendas, a coluna IDADE muda para NASC e usa o ano de nascimento.

## Snapshot de elencos
Dados atuais tratados como snapshot de 22/09/2026. Camisas não confirmadas na curadoria ficam como `null`/“—”, para não inventar informação.
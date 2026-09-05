# RPG WhatsApp Bot V3 — Escola, Progressão e Combate

Base para GitHub + Render. O motor é autoritativo: a IA/WhatsApp pode interpretar mensagens, mas regras, dano, XP, rank, requisitos e desbloqueios são calculados pelo servidor.

## Sistemas implementados
- Entrada automática de novos jogadores na Escola.
- Aulas: ataque, esquiva, bloqueio e habilidade.
- Teste final e liberação para jogo livre.
- Áreas protegidas por Rank e áreas exclusivas para administradores.
- Administrador recebe Rank S e acesso ao alto comando.
- XP, nível, atributos e promoção de Rank calculados automaticamente.
- Cards de batalha com elemento de cada jogador antes da luta.
- Esquiva e bloqueio com custo de fôlego.
- Bloqueio reduz o próximo dano em 60%.
- Validação de nível, Rank, Força, energia e fôlego para habilidades.
- Endpoint inicial de webhook do WhatsApp com verificação por token.

## Rodar no GitHub Codespaces
```bash
pip install -r requirements.txt
uvicorn app.main:app --host 0.0.0.0 --port 8080
```
Abra `/docs` para testar a API.

## Render
Configure as variáveis de ambiente. Para produção, use PostgreSQL; SQLite em serviço gratuito com disco efêmero não deve ser usado como banco persistente.

## Importante
Os números de Rank, XP, atributos, custos e elementos ainda são parâmetros configuráveis. Substitua-os pelos valores finais das cartas/regras do seu RPG.

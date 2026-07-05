# Mist-rios_em_S-rie
"Quero criar um jogo mobile de dedução lógica e mistério para jovens chamado 'Mistérios em Série'. O jogo deve ter múltiplos temas, fases progressivas e um MODO INFINITO que reinicia com modificadores de dificuldade.

Siga estritamente este raciocínio lógico estruturado para programar o jogo:

1. BANCO DE DADOS DE TEMAS (AS VARIAÇÕES):
Crie uma lista de objetos contendo pelo menos 5 temas diferentes para o mistério:
- Tema 1 (O Bolo): Suspeitos: [Irmão, Cachorro, Prima, Tio] | Locais: [Cozinha, Sala, Quintal, Varanda] | Pistas: [Pegada, Farelo, Pelo, Guardanapo]
- Tema 2 (A Escola): Suspeitos: [Zelador, Diretor, Aluno, Professora] | Locais: [Diretoria, Laboratório, Quadra, Biblioteca] | Pistas: [Óculos, Bilhete, Chaveiro, Caneta]
- Tema 3 (O Parque): Suspeitos: [Palhaço, Mágico, Pipoqueiro, Guarda] | Locais: [Carrossel, Roda-Gigante, Circo, Lago] | Pistas: [Balão, Ingresso, Pipoca, Cartola]
- Tema 4 (O Pet Shop): Suspeitos: [Gato, Furão, Papagaio, Hamster] | Locais: [Gaiola, Banho, Vitrine, Estoque] | Pistas: [Ração, Brinquedo, Pena, Coleira]
- Tema 5 (O Acampamento): Suspeitos: [Monitor, Instrutor, Guia, Colega] | Locais: [Barraca, Fogueira, Trilha, Rio] | Pistas: [Lanterna, Bússola, Mapa, Cantil]

2. SISTEMA DE PROGRESSÃO E LOOP INFINITO:
- O jogo começa no Nível 1 com o Tema 1.
- Quando o jogador acerta o mistério, ele avança para o próximo Tema (Fase).
- LOOP INFINITO: Quando o jogador vencer o último Tema da lista (ex: Tema 5), o jogo NÃO acaba. Ele volta automaticamente para o Tema 1, mas o contador global de 'CICLO' aumenta em +1 (Ciclo 2, Ciclo 3, etc.).

3. MODIFICADORES DE DIFICULDADE (MUDANÇAS SUTIS POR CICLO):
Toda vez que o Ciclo aumentar, mude as regras dinamicamente usando estas variáveis controladas pelo código:
- Ciclo 1: O jogador começa com 6 tentativas de palpite e 2 pistas reveladas de graça no início.
- Ciclo 2 (Modificador de Pistas): O jogador começa com 5 tentativas e apenas 1 pista revelada de graça.
- Ciclo 3 (Modificador de Tempo/Penalidade): O jogador começa com 4 tentativas, nenhuma pista revelada de graça, e cada palpite errado custa mais tempo no cronômetro.
- Ciclo 4 em diante: As listas de Suspeitos/Locais ganham 1 item genérico extra falso (aumentando a matriz de possibilidades de adivinhação).

4. MECÂNICA DE PALPITES:
- Em cada nível, sorteie 1 Suspeito, 1 Local e 1 Pista secretos do tema atual.
- O jogador faz o palpite. Se errar, o jogo desconta 1 tentativa e revela um dos itens que NÃO faz parte do mistério secreto para ajudá-lo a eliminar opções.

Com base nesta lógica de progressão infinita, loops de fases e modificadores de dificuldade por ciclo, gere o código completo do app mobile."

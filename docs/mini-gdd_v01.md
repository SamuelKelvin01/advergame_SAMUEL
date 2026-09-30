# Mini Game Design Document (Mini-GDD) - EcoCatch

## 1. Visão Geral
*EcoCatch* é um advergame 3D de captura horizontal para a marca EcoGuaraná[cite: 2]. O objetivo é reciclar o maior número de latinhas de alumínio e engajar o público com a sustentabilidade da marca[cite: 2].

## 2. Público e Plataforma
Desenvolvido para leitores e jogadores casuais de todas as idades[cite: 2]. Funciona diretamente no navegador web (HTML5 / Three.js) para telemóveis e computadores[cite: 2].

## 3. Core Loop
Objetos caem do topo -> Jogador move a lixeira verde -> Coleta latinhas de EcoGuaraná (+10 pts) / Desvia de lixo (-1 vida) -> Mudança de fases por pontuação -> Ganha o cupom promocional `RECICLA15`[cite: 2].

## 4. Mecânicas e Regras
Modo arcade de sobrevivência com 3 vidas[cite: 2]. O jogo termina quando as vidas chegam a 0[cite: 2]. Perde-se 1 vida ao apanhar lixo ou deixar uma latinha cair[cite: 2]. Colisão facilitada com raio de acerto amplo (hitbox 2.0)[cite: 2].

## 5. Mascote e Personagens
A Lixeira Verde 3D de Reciclagem é o elemento controlado pelo jogador[cite: 2]. O produto central é a Lata 3D de EcoGuaraná com rótulo verde[cite: 2].

## 6. Interface (UI)
Menu inicial de boas-vindas com tabela explicativa de itens e botão "JOGAR / START"[cite: 2, 3]. Na partida: placar de pontos, indicador de vidas e selo da fase atual[cite: 2]. Tela final de Game Over com o cupom de desconto[cite: 2, 3].

## 7. Direção de Arte e Paleta
Estilo 3D limpo e vibrante em ambiente urbano[cite: 2]. Cores da marca: Verde Reciclagem (`#27ae60`), Amarelo Energia (`#f1c40f`), Laranja Entardecer (`#e67e22`) e Roxo Noturno (`#1a252f`)[cite: 2].

## 8. Efeitos Visuais e Sonoros (VFX/SFX)
Efeitos visuais de explosão de partículas brilhantes ao coletar latinhas e tremor de câmara (*screen shake*) ao colidir com lixo[cite: 2]. Áudio procedural nativo via Web Audio API para sons de coleta, dano e fim de jogo[cite: 2].

## 9. Estratégia de Marketing (CTA)
Conversão direta em vendas no e-commerce da marca através do cupom `RECICLA15` exibido no ecrã de encerramento[cite: 2].
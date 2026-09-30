# Relatório Final de Desenvolvimento: EcoCatch

## 1. Resumo da Campanha
O *EcoCatch* é um advergame 3D casual desenvolvido para a marca EcoGuaraná com o objetivo de conscientizar o público sobre o descarte correto de latinhas de alumínio[cite: 2]. A experiência é executada diretamente no navegador sem necessidade de instalação e recompensa o engajamento do jogador com o cupom de desconto `RECICLA15` para conversão em vendas no e-commerce da marca[cite: 2].

## 2. Decisões Criativas
- **Mecânica Arcade (Catch Game):** A mecânica de coleta horizontal foi escolhida por ser altamente intuitiva, sem curva de aprendizado e funcional tanto em ecrãs táteis quanto no teclado[cite: 2].
- **Lixeira e Lata 3D:** Foco direto nos elementos do produto (lata de EcoGuaraná) e da sustentabilidade (lixeira verde de reciclagem)[cite: 2].
- **Cenário Evolutivo:** Transição visual entre Dia (Fase 1), Pôr do Sol (Fase 2) e Noite (Fase 3) para dar sensação dinâmica de progresso com base na pontuação atingida[cite: 2].

## 3. Integração da Marca
Nível **Demonstrativo**. A lata de EcoGuaraná é o elemento central coletável da partida e a jogabilidade simula diretamente o ato de reciclagem do produto[cite: 2].

## 4. Testes com Usuários
| Usuário | Compreensão | Dificuldade | Visual 3D | Controles | Recompensa / CTA |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **Usuário 1** | Entendeu as regras em menos de 5 segundos | Início calmo e acessível na Fase 1 | Elogiou a mudança de cor do céu entre fases | Achou muito fácil arrastar o dedo no telemóvel | Achou o cupom de 15% um excelente incentivo |
| **Usuário 2** | Entendeu o objetivo de primeira | Ritmo equilibrado e desafiador | Gostou do efeito de partículas ao coletar | Movimentação fluida e rápida no teclado | Pretende utilizar o desconto na loja online |

## 5. Orçamento Real (Uso de Recursos e IA)
| Ferramenta / Recurso | Quantidade / Iterações | Finalidade no Projeto |
| :--- | :--- | :--- |
| **Google AI Studio / Gemini** | 12 Gerações | Estruturação da lógica do jogo em Three.js, sintetizador Web Audio API e documentação |
| **Iterações de Renderização 3D** | 8 Iterações | Calibração de iluminação, sombras, sistema de partículas e hitbox facilitada (raio 2.0) |
| **Testes de Usabilidade / Ajustes** | 4 Iterações | Rebalanceamento do ritmo inicial das latinhas e criação da tela de menu inicial |

## 6. O que deu errado e como resolveu
1. **Colisão inicial muito rígida:** A área de acerto da lixeira exigia precisão excessiva. **Solução:** Ampliou-se o raio de colisão da hitbox para `2.0`, permitindo coletar a lata mesmo encostando de raspão.
2. **Ritmo de queda muito acelerado no início:** Caíam muitas latinhas logo no começo da partida. **Solução:** A Fase 1 foi rebalanceada para uma velocidade suave (`0.07`) com intervalo maior entre objetos (`900ms`).
3. **Lentidão ao segurar as setas do teclado:** Havia atrito e atraso de repetição do sistema operativo. **Solução:** Mapeou-se o estado contínuo das teclas com escuta de `keydown` e `keyup`, garantindo movimentação instantânea.

## 7. Declaração de Uso de IA
- **Ferramentas Utilizadas:** Google AI Studio / Gemini para auxílio técnico na programação em JavaScript com Three.js e rascunho de estrutura documental.
- **Decisões Curadas por Humanos:** Conceituação da campanha de marketing, regras do cupom promocional `RECICLA15`, sistema de 3 vidas, curva de dificuldade das 3 fases e direção de arte final[cite: 2].
# GS---Edge-Computing

# Flood360: Sistema de Monitoramento de Enchentes

## 🌊 Descrição do Problema

As enchentes estão entre os desastres naturais mais comuns no Brasil, afetando milhares de pessoas todos os anos. A falta de sistemas de alerta precoce agrava a situação, já que muitos moradores não têm tempo suficiente para evacuar ou se preparar adequadamente.

### Impactos das Enchentes
- 🧍‍♂️ **Perdas humanas**: mortes e ferimentos causados por inundações repentinas  
- 🏚️ **Danos materiais**: destruição de residências, comércios e infraestrutura  
- 💸 **Impacto econômico**: prejuízos de bilhões de reais anualmente  
- 🦠 **Problemas de saúde**: doenças transmitidas por água contaminada  

### Desafios Atuais
- Falta de monitoramento em tempo real em áreas vulneráveis  
- Ausência de sistemas de alerta acessíveis para comunidades de baixa renda  
- Dificuldade na comunicação rápida e eficiente em situações de emergência  

---

## ✅ Visão Geral da Solução

O **Flood360** é um sistema de monitoramento e alerta de enchentes baseado em **Arduino**, que mede em tempo real o nível da água e emite **alertas progressivos** conforme o risco aumenta. Utiliza sensores e componentes simples, tornando-se acessível e eficaz.

---

## 🔧 Componentes Principais

- **Arduino Uno**: Unidade de controle do sistema  
- **Sensor Ultrassônico HC-SR04**: Mede a distância da água até o sensor  
- **Display LCD 16x2**: Exibe o nível da água e mensagens de alerta  
- **LEDs Coloridos**: Indicação visual dos níveis de risco  
- **Buzzer**: Emite sinais sonoros de alerta  

---

## 🚦 Níveis de Alerta

| Distância (cm) | Nível               | LED     | Alerta Sonoro     | Mensagem LCD                     |
|----------------|---------------------|---------|--------------------|----------------------------------|
| > 180          | Seguro              | Branco  | Nenhum             | "Nível Seguro"                   |
| 136 – 180      | Normal              | Verde   | Nenhum             | "Nível Normal"                   |
| 91 – 135       | Acima do Normal     | Amarelo | Nenhum             | "Nível Acima do Normal"          |
| 46 – 90        | Alerta              | Vermelho| Contínuo           | "!!! ALERTA !!!"                 |
| < 45           | Perigo/Evacuação    | Vermelho| Contínuo           | "!!! PERIGO !!!" / "!!! EVACUAR !!!" |

---

## 💡 Diferenciais do Sistema

- 🎨 **Logo personalizada**: Tela de abertura com logo animada do Flood360  ![image](https://github.com/user-attachments/assets/8af0bb0e-db68-47d6-b9d8-dfdece083ca9)
- 📊 **Indicadores dinâmicos**: Ícones especiais no LCD mudam conforme o nível de alerta  
- 🔁 **Mensagens alternadas**: Em perigo, LCD alterna entre "PERIGO" e "EVACUAR"  
- 🔉 **Padrões sonoros inteligentes**: Alertas sonoros distintos por nível de risco  

---

## 🧪 Guia para Simulação no Tinkercad

### Passo 1: Acessar o Projeto
1. https://www.tinkercad.com/things/4AausHw8A5O-gs-edge-computing-e-iot?sharecode=4qm6pzGXqzPYyh4THnVr1Y5vqGG-YAjmrjNlzHC6qlo
2. Faça login ou crie uma conta no Tinkercad  
3. Clique em **"Tinker this"** para editar/simular

---

### Passo 2: Entendendo o Circuito

- Imagem Circuito: ![GS - Edge Computing e IoT](https://github.com/user-attachments/assets/900d8555-bcdb-4fea-ab0c-099d807cbbe9)

- **Arduino Uno**: Placa principal  
- **Sensor Ultrassônico HC-SR04**:  
  - TRIG → Pino 8  
  - ECHO → Pino 9  
- **Display LCD 16x2**:  
  - RS, E, D4–D7 → Pinos 2, 3, 4, 5, 6, 7  
- **LEDs**:  
  - Branco (Seguro) → Pino 13  
  - Verde (Normal) → Pino 12  
  - Amarelo (Acima do normal) → Pino 11  
  - Vermelho (Alerta/Perigo) → Pino 10  
- **Buzzer**: Pino 7  



---

### Passo 3: Executando a Simulação

1. Clique em **"Start Simulation"**  
2. Veja a tela inicial com logo animada  
3. Use a ferramenta de mão para mover um objeto em direção ao sensor e simular o aumento da água  
4. Observe a resposta do sistema: mudança de LEDs, mensagens no LCD e som do buzzer  

---

### Passo 4: Testando os Níveis de Alerta

- **> 180 cm** → Nível Seguro  
- **136 – 180 cm** → Nível Normal  
- **91 – 135 cm** → Acima do Normal  
- **46 – 90 cm** → Alerta  
- **< 45 cm** → Perigo / Evacuação  


---

## 📸 Vídeo para Simulação no Tinkercad

### Link para o Vídeo no Youtube: https://youtu.be/Z4paZNDwAtc?si=oOwCXiMrJQTGJCUu

---

## 👨‍🔬 Desenvolvido por

**Sebastian Iriarte Gonzales** – RM 563619 - Engenharia de Software – FIAP  
**Fabio Pereira Rogério Júnior** - RM 564005 - Engenharia de Software – FIAP  
Projeto para a disciplina de **Edge Computing & IoT (Global Solution 2025.1)**  

---

## 📬 Contato

Caso tenha dúvidas ou sugestões, sinta-se à vontade para abrir uma issue ou entrar em contato.



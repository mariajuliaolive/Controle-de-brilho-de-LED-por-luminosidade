 Projeto: Controle de brilho de LED por luminosidade

![Status](https://img.shields.io/badge/status-concluído-brightgreen)

Este projeto utiliza um Arduino para controlar a intensidade de um LED com base na luminosidade do ambiente, capturada por um sensor LDR. Funciona como uma luz de presença automática: acende no escuro e apaga no claro, de forma proporcional.

---

##  기능 (Funcionalidades)

- **Controle automático de brilho:** A intensidade do LED é ajustada automaticamente de acordo com a luz ambiente.
- **Lógica de controle inversa:** Quanto mais escuro o ambiente, mais forte o LED brilha.
- **Monitoramento em tempo real:** Envia dados detalhados para o Monitor Serial do Arduino, incluindo intensidade da luz (%), resistência do LDR (Ohms) e o valor PWM enviado ao LED.

---

## Hardware Necessário

| Componente | Quantidade |
| :--- | :---: |
| Arduino Uno (ou similar) | 1 |
| Protoboard | 1 |
| LED (qualquer cor) | 1 |
| Sensor LDR | 1 |
| Resistor de 220Ω | 1 |
| Resistor de 10kΩ | 1 |
| Jumpers (fios de conexão) | Vários |

---

## Esquema do Circuito

> **Nota:** Para que a imagem apareça, você precisa primeiro fazer o upload dela para o seu repositório e depois substituir o `link_da_sua_imagem_aqui.png` pelo link correto.

![Esquema do Circuito](link_da_sua_imagem_aqui.png)

---

## Como Usar

1.  **Monte o circuito** na protoboard conforme o esquema acima.
2.  **Conecte o Arduino** ao seu computador via USB.
3.  **Abra o código-fonte** (`.ino`) na IDE do Arduino.
4.  **Verifique a constante `RESISTOR_FIXO`** no código. Certifique-se de que o valor (padrão `10000.0`) corresponde ao resistor que você usou em série com o LDR.
5.  **Carregue (upload) o código** para a placa Arduino.
6.  **Abra o Monitor Serial** (`Ferramentas > Monitor Serial`) com a velocidade de **9600 baud** para visualizar as leituras do sensor em tempo real.
7.  Cubra o LDR com a mão ou aponte uma luz para ele para ver o brilho do LED e os dados no monitor mudarem.

---

## Código-Fonte

O código principal do projeto pode ser encontrado no arquivo `principal` deste repositório.


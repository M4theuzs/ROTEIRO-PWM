# Arduino PWM Controller

## 1. Introdução

O PWM é uma forma de controlar a velocidade de um motor usando sinais digitais do Arduino. Neste projeto, o motor aumenta a velocidade cada vez que o botão é pressionado.

---

## 2. Componentes Utilizados

* Arduino Nano
* CI L293D
* Motor DC
* Botão
* Resistor 10kΩ
* Bateria/Fonte 5V

---

## 3. Esquemático

O circuito foi montado no Proteus.
O Arduino envia o sinal PWM para o L293D, que controla o motor DC.

O arquivo do esquema está na pasta:

```bash
/schematics
```

---

## 4. Código

O código foi feito no VS Code com PlatformIO.

A função utilizada para controlar a velocidade do motor foi:

```cpp
analogWrite()
```

Arquivo principal:

```bash
/src/main.cpp
```

---

## 5. Funcionamento

* O motor inicia desligado;
* Cada clique no botão aumenta a velocidade;
* Os níveis são:

  * 25%
  * 50%
  * 75%
  * 100%
* Depois disso, o motor volta para 0%.

---

## 6. Conclusão

O projeto mostrou como usar PWM no Arduino para controlar a velocidade de um motor DC de forma simples usando um botão e o driver L293D.

# Apresentação do Projeto – Monitoramento do Nível do Rio

Olá, somos uma equipe contratada por uma startup de monitoramento ambiental e viemos apresentar nosso projeto sobre o **monitoramento do nível do rio e planejamento de evacuação** em períodos de chuva intensa.

---

## 1. Contexto

A cidade escolhida foi **Santo André (SP)**, conhecida por enfrentar enchentes com frequência. Nosso objetivo foi criar uma **função matemática** que represente o comportamento do nível de um rio durante 10 dias consecutivos de chuva.

---

## 2. Dados Coletados (Simulados)

Coletamos e simulamos os seguintes dados de nível do rio:

| Dia | Nível (m) |
| --- | --------- |
| 1   | 0.5       |
| 2   | 0.9       |
| 3   | 1.4       |
| 4   | 1.9       |
| 5   | 2.3       |
| 6   | 2.7       |
| 7   | 2.9       |
| 8   | 2.8       |
| 9   | 2.4       |
| 10  | 2.0       |

---

## 3. Modelagem Matemática

Utilizamos uma **função polinomial de grau 2** para aproximar o comportamento do rio:

$f(x) = -0.064x^2 + 0.917x - 0.583$

Onde $x$ representa o dia, e $f(x)$, o nível do rio em metros.

---

## 4. Análise da Função

* **Domínio:** $x \in [1, 10]$ → dias observados
* **Imagem:** $f(x) \in [0.5, 2.9]$ → variação do nível
* **Pico:** Dia 7, com **2.9m**
* **Risco de transbordamento (> 2m):** Dias 5, 6, 7, 8 e 9

---

## 5. Aplicação Prática

Esse modelo pode ser aplicado em sistemas de alerta preventivo para:

* Acionar evacuações em áreas críticas
* Alertar a defesa civil com antecedência
* Comunicar a população com previsões precisas

---

## 6. Protótipo Digital

Criamos um conceito de sistema visual que apresenta a curva do nível do rio ao longo dos dias e uma classificação baseada em faixas de risco:

* **Seguro:** Nível < 1.5m
* **Atenção:** 1.5m a 2.0m
* **Risco de enchente:** > 2.0m

Esse painel pode ser alimentado por sensores físicos ou dados de API, aplicando nossa equação para prever os níveis futuros.

### Imagem do Protótipo

![image](https://github.com/user-attachments/assets/90be2fc5-5cf8-46fc-b10a-3f5ed5872a7f)


---

## 7. Conclusão

Com essa função polinomial e seu uso integrado a um sistema digital, conseguimos antecipar enchentes, minimizar riscos e aumentar a segurança da população em áreas vulneráveis.

Obrigado!

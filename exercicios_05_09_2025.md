# Linguagens_Formais-UNIALFA
> Atividades de Linguagens Formais e Autômatos - UNIALFA - exercicios_05_09_2025

# Questões sobre o Processo de Compilação em Java

## 1. Diferença entre compilação em Java e C++
- **C++:** compila diretamente para código de máquina específico do sistema operacional e do hardware. O resultado é um executável nativo.  
- **Java:** compila para **bytecode**, um código intermediário independente de plataforma, que será executado pela JVM.  

---

## 2. Fases de análise do compilador `javac`
- **Análise Léxica:** converte o código-fonte em tokens (identificadores, palavras-chave, símbolos).  
- **Análise Sintática:** verifica se a sequência de tokens segue as regras da gramática da linguagem (estrutura correta do programa).  
- **Análise Semântica:** checa o significado dos elementos, como compatibilidade de tipos e declarações de variáveis.  

---

## 3. O que é o bytecode
É o código intermediário gerado pelo compilador Java (`.class`).  
**Função principal:** permitir que o mesmo programa seja executado em qualquer sistema que tenha a JVM, garantindo portabilidade.  

---

## 4. Papel da JVM e execução do `.class`
- A **JVM** interpreta ou compila em tempo de execução o bytecode para instruções da máquina real.  
- O arquivo `.class` não roda diretamente no SO porque não contém instruções nativas, apenas o bytecode, que precisa da JVM para ser traduzido.  

---

## 5. Compilador JIT
O **Just-In-Time Compiler (JIT)** converte partes do bytecode em código de máquina enquanto o programa está sendo executado.  
**Vantagem:** aumenta o desempenho, já que o código traduzido pode ser reutilizado sem precisar ser interpretado novamente.  

---

# Questões sobre Linguagens Formais em Java

## 6. Aplicação das linguagens formais em Java
A aplicação mais comum é na **definição da sintaxe da linguagem**.  
São usadas para criar e validar regras que estruturam o código-fonte, garantindo que ele seja corretamente interpretado pelo compilador.  

---

## 7. Uso nas fases de compilação
- **Análise Léxica:** linguagens formais (expressões regulares) definem os padrões de tokens válidos.  
- **Análise Sintática:** gramáticas formais (como gramáticas livres de contexto) descrevem a estrutura do código e são usadas para construir a árvore sintática.  

---

## 8. Máquina de Estado Finito (FSM) em Java
Uma FSM é um modelo que representa estados e transições.  
Em Java, pode ser usada para:  
- Validar entrada de dados,  
- Controlar fluxos de protocolos de comunicação,  
- Modelar comportamento de jogos ou sistemas reativos.  

---

## 9. Relação com validação de XML e JSON
As linguagens formais permitem descrever **schemas** (regras de estrutura e formato).  
Exemplo: XML Schema (XSD) e JSON Schema garantem que os documentos sigam uma gramática bem definida.  

---

## 10. Utilidade do ANTLR
Ferramenta usada para **gerar analisadores léxicos e sintáticos**.  
No contexto de Java, facilita a criação de compiladores, interpretadores ou validadores de linguagens específicas, automatizando parte do trabalho de análise de código.  

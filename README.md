# 🎈 Decor Puf - Sistema de Gerenciamento Comercial (Front-end)

> **⚠️ Status do Projeto:** Este repositório apresenta **exclusivamente a minha contribuição** para um projeto acadêmico em grupo do curso de Ciência da Computação. O código disponibilizado aqui é focado 100% no **Front-end (Interface Gráfica) e Lógica de Validação**. A persistência de dados (conexão com Banco de Dados) será integrada pela equipe nas próximas etapas.

Este é um sistema desktop desenvolvido para o gerenciamento interno de uma loja de adereços de festas. Como desenvolvedor responsável pela engenharia da Interface Gráfica (GUI), meu objetivo foi construir uma aplicação amigável e blindada contra falhas de operação, garantindo a integridade dos dados inseridos pelo usuário antes do envio para o servidor.

## 💻 Telas Desenvolvidas (Até o momento)

### 🔒 Autenticação (Login)
Módulo de segurança para controle de acesso restrito, diferenciando as permissões entre atendentes e gerentes.
* **UX/UI Dinâmica:** A interface inicializa automaticamente em modo Tela Cheia (`MAXIMIZED_BOTH`). Utilizei `GridBagLayout` combinado com `JPanel` para garantir que o formulário de login permaneça perfeitamente centralizado, independentemente da resolução do monitor.

<img width="662" height="439" alt="image" src="https://github.com/user-attachments/assets/7ceaf05b-77c2-40ea-9135-692c06d3f9af" />
<img width="673" height="445" alt="image" src="https://github.com/user-attachments/assets/ffd6e885-b88c-444e-ba54-9bd5a448eb0f" />


---

### 👥 Cadastro de Clientes
Formulário robusto para o registro seguro de novos clientes, focado em evitar a inserção de dados "sujos" no sistema.
* **Máscaras de Entrada:** Utilização nativa de `JFormattedTextField` para formatação em tempo real e bloqueio de caracteres alfabéticos em campos sensíveis (CPF e Telefone).
* **Validações Lógicas Avançadas:**
  * Bloqueio de números no campo "Nome" utilizando Expressões Regulares (**Regex**: `.*\\d.*`).
  * Validação de estrutura obrigatória para E-mails (presença de `@` e `.`).
  * Higienização de Strings (métodos `.trim()` e `.replace()`) para limpar espaços em branco indesejados antes da checagem de limites.
* **Proteção de Layout:** Definição de tamanhos absolutos (*Minimum/Maximum Size*) nos painéis para evitar que o disparo de alertas (`JOptionPane`) quebre o alinhamento visual durante o uso.

<img width="913" height="468" alt="image" src="https://github.com/user-attachments/assets/c0432b3f-5252-4cfa-bcd6-b88de52487ea" />
<img width="729" height="426" alt="image" src="https://github.com/user-attachments/assets/014b4ece-a3b1-4189-b882-2c9724fa3e24" />
<img width="870" height="416" alt="image" src="https://github.com/user-attachments/assets/ce40059a-ffdb-4023-88c7-5170134c05b8" />


---

### 📦 Cadastro de Produtos (Uso Gerencial)
Tela dedicada à expansão do catálogo da loja, manipulando dados financeiros, controle de estoque inicial e arquivos de imagem.
* **Upload Dinâmico de Imagens:** Implementação de `JFileChooser` com filtros para extensões específicas (`.jpg`, `.png`). Utilizei cálculo de *Aspect Ratio* via `Image.SCALE_SMOOTH` para redimensionar as fotos inseridas sem causar distorção visual na interface.
* **Regras de Negócio de Interface:** * Uso de `JSpinner` com modelo numérico restrito para impedir o cadastro de estoque negativo.
  * Implementação de `JCheckBox` para o gerente definir a modalidade do produto (Aluguel, Venda ou Ambos).
* **Tratamento Financeiro Seguro:** O campo de Valor converte e limpa automaticamente os separadores de milhar visuais no momento do cadastro, garantindo a conversão perfeita para ponto flutuante (`Double`) exigida pelo Java.

<img width="978" height="596" alt="image" src="https://github.com/user-attachments/assets/afe3607b-875a-4640-8428-4cf58433c03a" />
<img width="959" height="527" alt="image" src="https://github.com/user-attachments/assets/32007169-847c-47d0-91ed-8a4a796ac7f7" />
<img width="888" height="528" alt="image" src="https://github.com/user-attachments/assets/b5e3fc01-244e-4514-8e70-4fc897950c86" />




## 🛠️ Tecnologias e Ferramentas

* **Linguagem:** Java (Orientação a Objetos)
* **Interface Gráfica (GUI):** Java Swing
* **IDE:** Apache NetBeans (GUI Builder)
* **Arquitetura:** Componentização de layouts (`GridBagLayout` e `Free Design`), tratamento avançado de Exceções (`try-catch`) e manipulação de arquivos (I/O).

---
Desenvolvido com dedicação por **Maasayoshii** 🚀

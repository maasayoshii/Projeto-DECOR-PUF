# Projeto-DECOR-PUF
No trabalho da faculdade fiquei responsavel pela parte de Login e Cadastro de Cliente.
Um sistema desktop desenvolvido em Java para o gerenciamento interno de uma loja de adereços de festa. Este projeto foi focado na criação de uma interface gráfica amigável e segura para os atendentes, garantindo a integridade dos dados antes mesmo de chegarem ao banco de dados.

## 💻 Funcionalidades Atuais

* 🔒 Tela de Autenticação (Login):
    * Controle de acesso restrito para atendentes e gerentes.
    * Interface responsiva que inicializa automaticamente em modo Tela Cheia (`MAXIMIZED_BOTH`), centralizando os componentes dinamicamente com `GridBagLayout`.
*   👥 **Cadastro de Clientes:** * Formulário robusto para registro de novos clientes (Nome, E-mail, CPF, Telefone).
    * **Máscaras de Entrada:** Utilização de `JFormattedTextField` para formatação automática e bloqueio de caracteres inválidos em campos sensíveis (CPF e Telefone).
    * **Validações Avançadas de Lógica:**
        * Bloqueio de números no campo de Nome utilizando Expressões Regulares (**Regex**: `.*\\d.*`).
        * Verificação de limite máximo (100) e mínimo (3) de caracteres.
        * Validação de formatação obrigatória para o E-mail (presença de `@` e `.`).
        * Tratamento de Strings (`.trim()`, `.replace()`) para limpar dados de entrada antes da checagem.
    * **Proteção de Layout:** Aplicação de tamanhos absolutos (Minimum, Maximum e Preferred Size) em painéis agrupados para garantir que alertas de erro (`JOptionPane`) não quebrem o alinhamento da interface durante o *repaint* da tela.
 
    * 🛠️ Tecnologias e Ferramentas

* Linguagem: Java
* Interface Gráfica: Java Swing
* IDE Gráfica: Apache NetBeans

  * 📸 Capturas de Tela
* <img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/39c4ecd5-4055-4b73-9907-f240650ce066" />
* <img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/dbf26bf8-af92-4d81-b182-9b617eb60634" />
* <img width="500" height="300" alt="image" src="https://github.com/user-attachments/assets/1db530fb-ed3f-451f-83ea-cb7cd82a704e" />
* <img width="365" height="390" alt="image" src="https://github.com/user-attachments/assets/c2634422-9309-4ee1-89ec-b27f0099cc11" />
* <img width="500" height="425" alt="image" src="https://github.com/user-attachments/assets/a33e3e14-0852-42b8-a713-058848ad92d9" />
* <img width="863" height="471" alt="image" src="https://github.com/user-attachments/assets/a239d56d-8931-458b-a2b4-fed90290897f" />



# :balance_scale: LegisFlow Cartório
> **Portal de Atualização Normativa e Gestão de Conhecimento**

Este projeto foi desenvolvido como parte da disciplina **Fundamentos de No-code e Low-code** da UniFECAF em parceria com a Rocketseat.

>O desafio consiste em criar uma aplicação web funcional no Bubble que resolve um problema real de gestão de tarefas. O produto é um portal de gerenciamento de tarefas e comunicação interna, onde times colaboram, criam e atualizam tarefas com comentários e notificações. 

O **LegisFlow** é uma aplicação web desenvolvida para otimizar a gestão normativa dentro de um Registro de Imóveis. O projeto visa substituir fluxos informais de comunicação (WhatsApp/E-mail) por uma plataforma centralizada que garante a ciência inequívoca de provimentos, decisões e leis pelos escreventes.

![LEGISFLOW](https://github.com/brugaby2342/legisflow/blob/main/assets/bubble%20_dash.png)


## 📝 O Problema
No ambiente registral, a atualização legislativa e afins é diária e obrigatória. Porém, o uso de canais informais de comunicação, como WhatsApp e e-mail, gera dispersão de dados e não oferece ao Oficial a possibilidade de fiscalização quanto a ciência de toda a equipe. Além disso, é sentida a falta de um repositório centralizado para consulta.

## 🚀 A Solução
O **LegisFlow** oferece:
- **Para o Escrevente:** Dashboard com lista de normas pendentes, leitura de PDF integrada e fórum de debates.
- **Para o Oficial:** Cadastro de normas em "Cards", anexos de arquivos e uma **Tabela de Conformidade** para monitoramento.

## :on: Fluxo Básico da Aplicação:
1. **Cadastro de Tarefa:** O Oficial cadastra uma nova norma.
2. **Checklist de Ciência:** Cada escrevente visualiza o PDF e marca como "Ciente e Lido".
3. **Fórum Técnico:** Discussões práticas sobre a norma ocorrem abaixo do documento, centralizando o aprendizado.
4. **Dashboard Gerencial:** Barra de progresso visual que mostra o percentual de leitura da equipe.

## 🛠️ Tecnologias Utilizadas
- **Plataforma:** Engine principal para desenvolvimento No-code.
- **Metodologia:** Desenvolvimento Visual de Software
- **Workflow Logics:** Automação de cálculos de progresso e regras de privacidade (Privacy Rules).

## 🗄️ Arquitetura de Dados (Relacional)
O sistema utiliza um modelo relacional para garantir a integridade:
- **User:** Dados de autenticação, nome e Cargo (Option Set).
- **Norma:** Título, descrição, arquivo PDF.
- **Confirmação da Leitura:** Tabela de ligação que registra a leitura individual de cada usuário.
- **Comentário:** Relaciona o autor à norma, permitindo o fórum interno.

## ⚡ Principais Workflows
- **Lógica de Ciência:** Criação dinâmica de registros na tabela `Ciência` ao clique do usuário.
- **Cálculo de Progresso:** Expressão matemática em tempo real: `(Total de Ciências do Usuário / Total de Normas) * 100`.
- **Filtros Inteligentes:** **Triagem Rápida:** Filtros dinâmicos para Normas Lidas e Não Lidas.
- **Identidade Visual:** Aplicação dinâmica de cores baseada no Cargo do usuário.
- **KPI Cards:** Indicadores de produtividade no topo do Dashboard.
- **Segurança:** Regras de privacidade que protegem dados sensíveis conforme a hierarquia do cartório.

## :lock: Privacidade
- Dois níveis de acesso:
  - Dashboard do Escrevente: Focado em produtividade e leitura.
  - Painel Administrativo: Focado em gestão, cadastro e fiscalização (*Compliance*).
- Lógica de redirecionamento.
- Acessos bloqueados.

## 🎨 Interface e Usabilidade (UX/UI)
**Design:** 
- O azul marinho remete à sobriedade do Direito e dos Registros Públicos.
- As etiquetas mudam de cor e estado assim que o usuário confirma a leitura.

## 🔗 Acesse e teste o **LegisFlow** através do link da aplicação:
[LegisFlow](https://gabrielarsartor-27255.bubbleapps.io/version-test)

> Cadastre-se e faça log-in. Na página principal (Dashboard), você terá acesso às normas recentemente publicadas pelo Oficial. Você pode dar seu ciente e comentar. Pela side bar, através do menu, terá a opção de acessar a biblioteca de normas, onde encontrará o histórico de publicações e seu progresso nas leituras.
Observação: para ter acesso a menu "Admministrativo", terá que cadastrar direto no banco de dados, um user como Oficial. Nesta área, você poderá cadastrar novas normas e fiscalizar o processamento.

---

### 📖 [Documentação Acadêmica](https://github.com/brugaby2342/legisflow/blob/main/assets/Projeto%20Bubble.pdf)

---

### 👩‍💻 Desenvolvedora
**Bruna Gabriela Ribeiro Sartor** 
*Escrevente no Registro de Imóveis de Curitibanos/SC.  
Estudante de IA e Automação Digital.*

---
*Nota: Este projeto encontra-se em ambiente de versão-test (Development).*


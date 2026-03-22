# :balance_scale: LegisFlow Cartório
> **Portal de Atualização Normativa e Gestão de Conhecimento**

## PRINTS
![Bubble.io]()

Este projeto foi desenvolvido como parte da disciplina **Fundamentos de No-code e Low-code** da UniFECAF em parceria com a Rocketseat. O objetivo é resolver o "silêncio" dos sistemas oficiais de cartório, centralizando a gestão do conhecimento jurídico e garantindo a conformidade normativa.

## 📝 O Problema
No dia a dia do Ofício de Registro de Imóveis, novas normas (Provimentos do CNJ, decisões da CGFE/SC) surgem constantemente. A comunicação via WhatsApp ou e-mail gera dispersão de dados e não oferece ao Oficial uma prova de conformidade (compliance) de que toda a equipe foi devidamente cientificada.

## 🚀 A Solução
O **LegisFlow** permite que administradores cadastrem normas em "Cards", anexem arquivos e monitorem em tempo real quem já realizou a leitura. A plataforma transforma a atualização jurídica em um processo auditável e colaborativo.

### Fluxo Básico da Aplicação:
1. **Cadastro de Tarefa:** O Oficial cadastra uma nova norma.
2. **Checklist de Ciência:** Cada escrevente visualiza o PDF e marca como "Ciente e Lido".
3. **Fórum Técnico:** Discussões práticas sobre a norma ocorrem abaixo do documento, centralizando o aprendizado.
4. **Dashboard Gerencial:** Barra de progresso visual que mostra o percentual de leitura da equipe.

## 🛠️ Tecnologias Utilizadas
- **Plataforma:** [Bubble.io](https://bubble.io/) (No-code)
- **Metodologia:** Desenvolvimento Visual de Software
- **Layout:** Responsive Engine (Containers Row e Column)

## 🗄️ Arquitetura de Dados (Relacional)
A estrutura foi desenhada para suportar relacionamentos N:N (Muitos para Muitos) entre Usuários e Normas:

- **User:** Dados de autenticação, nome e Cargo (Option Set).
- **Norma:** Título, descrição, arquivo PDF.
- **Ciência:** Tabela de ligação que registra a leitura individual de cada usuário.
- **Comentário:** Relaciona o autor à norma, permitindo o fórum interno.

## ⚡ Principais Workflows
- **Lógica de Ciência:** Criação dinâmica de registros na tabela `Ciência` ao clique do usuário.
- **Cálculo de Progresso:** Expressão matemática em tempo real: `(Total de Ciências do Usuário / Total de Normas) * 100`.
- **Filtros Inteligentes:** Busca por título e filtragem por status (Lido/Pendente) utilizando a lógica de *Ignore empty constraints*.
- **Identidade Visual:** Aplicação dinâmica de cores baseada no Cargo do usuário.

## 🎨 Interface e Usabilidade (UX/UI)
- **Hierarquia Visual:** O azul marinho remete à sobriedade do Direito e dos Registros Públicos.
- **Feedback Instantâneo:** As etiquetas mudam de cor e estado assim que o usuário confirma a leitura.
- **Responsividade:** Interface adaptável para uso em tablets (balcão) ou desktops.

## 🔗 Links do Projeto
- **Aplicação Funcional:** [Link do seu app no Bubble aqui]
- **Vídeo Pitch:** [Link do seu vídeo no Youtube/Loom aqui]

---
**Desenvolvido por Gabi** *Estudante de IA e Automação Digital - UniFECAF*


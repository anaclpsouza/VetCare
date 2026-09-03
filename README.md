# 🐾 VetCare — Clínica Veterinária

> Site institucional desenvolvido como atividade da PD Case para uma clínica veterinária, desenvolvido a partir de protótipo no Figma até a implementação em código com HTML5 semântico e CSS3 puro.

[![Figma](https://img.shields.io/badge/Figma-Protótipo%20do%20Projeto-F24E1E?style=for-the-badge&logo=figma&logoColor=white)](https://www.figma.com/design/sjeLJVeAr3zFq8qwjqYnZc/Cl%C3%ADnica-Veterin%C3%A1ria---VetCare?node-id=110-2973&t=qkqVRTceeRCfRyU7-1)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](#)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](#)

---

## 🎨 Protótipo no Figma

Acesse o design completo e o protótipo navegável diretamente no Figma:

🔗 **[Protótipo VetCare no Figma](https://www.figma.com/design/sjeLJVeAr3zFq8qwjqYnZc/Cl%C3%ADnica-Veterin%C3%A1ria---VetCare?node-id=110-2973&t=qkqVRTceeRCfRyU7-1)**

---

## 🎯 Objetivo da Tarefa

Construir o site institucional para a clínica veterinária **VetCare**, traduzindo o design concebido no Figma para código web semântico, acessível e responsivo para celulares, tablets e desktops.

### 🧭 Fluxo do Usuário

```text
Home (Início)
  ↓
Sobre a Clínica & Conheça a Estrutura
  ↓
Serviços Oferecidos
  ↓
Corpo Clínico (Veterinários)
  ↓
Perfil do Veterinário Selecionado & Agendamento
  ↓
Informações de Contato & Localização
```

---

## 📱 Telas e Funcionalidades

O projeto é composto por 7 páginas interligadas:

1. **Página Inicial (`index.html`)**:
   - Hero com chamada principal e botão de agendamento.
   - Apresentação em destaque dos serviços da clínica.
   - Banner institucional sobre a infraestrutura e bem-estar animal.
   - Seção de depoimentos de tutores estilizados como balões de fala.
   - Rodapé com links de navegação rápida, redes sociais e canais de atendimento.

2. **Sobre Nós (`pages/sobre.html`)**:
   - Cartões detalhando a História, a Missão e os Valores da clínica.
   - Banners de chamada para ação (CTAs) para conhecer a estrutura e o corpo clínico com ilustração temática.

3. **Nossos Serviços (`pages/servicos.html`)**:
   - Catálogo de procedimentos oferecidos: Consultas Clínicas, Exames Diagnósticos, Centro Cirúrgico, Odontologia Veterinária e Imunização/Microchipagem.
   - Links diretos para selecionar o médico veterinário de preferência.

4. **Estrutura da Clínica (`pages/estrutura.html`)**:
   - **Carrossel interativo** com navegação anterior/próximo construído exclusivamente em CSS (via seletores `:target`).
   - Galeria fotográfica em grade responsiva destacando o ambiente e os cuidados com os pets.
   - Botões de retorno e direcionamento para contato.

5. **Corpo Clínico (`pages/veterinarios.html`)**:
   - Exibição de cards de cada especialista (Medicina Felina, Cirurgia Geral, Odontologia, Dermatologia e Cardiologia).
   - Botão **Agendar** em cada profissional, direcionando com âncora para a ficha individual do veterinário.
   - Botão de filtro visual por especialidade.

6. **Agendamento & Perfil (`pages/agendamento.html`)**:
   - Exibição dinâmica da foto, biografia e credenciais do médico veterinário selecionado via URL hash (`:target` em CSS).
   - Formulário completo para solicitação de consulta (nome do tutor, pet, espécie, serviço, data, horário e sintomas).

7. **Contato (`pages/contato.html`)**:
   - Informações institucionais de atendimento (WhatsApp com link direto, endereço e horário de funcionamento).
   - Seção de contatos administrativos / trabalhe conosco com links funcionais (`tel:` e `mailto:`).
   - Mapa de localização interativo integrado via Google Maps iframe.

---

## 🛠️ Tecnologias Utilizadas

- **HTML5 Semântico**: Estruturação semântica e acessível utilizando tags como `<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<aside>`, `<address>` e `<footer>`.
- **CSS3 Moderno**:
  - Layouts flexíveis e responsivos construídos com **Flexbox** e **CSS Grid**.
  - Variáveis de cores e tipografia no `:root` (*Design System*).
  - Componentes interativos sem JavaScript (carrossel de imagens, menu hambúrguer mobile e alternância de perfis de agendamento via `:target`, `:has` e `:checked`).
  - **Design Responsivo**: Breakpoints otimizados para Mobile (<768px), Tablet (≥768px) e Desktop (≥1024px).
- **Iconografia & Tipografia**:
  - Font Awesome 6.5.1
  - Tipografia [Quicksand](https://fonts.google.com/specimen/Quicksand) via Google Fonts
  - Ícones e ilustrações vetoriais em formato SVG

---

## 🎨 Paleta de Cores (Design System)

| Cor | Hex | Uso |
| :--- | :--- | :--- |
| **Primary** | `#FFBBC1` | Navbar, cabeçalhos, destaques e cards |
| **Secondary** | `#6DB5D8` | Botões secundários, cards de serviços e veterinários |
| **Accents** | `#FF914D` | Botões de destaque, estrelas de avaliação e detalhes |
| **Accents Blue** | `#78B0B2` | Card de infraestrutura e serviços |
| **Neutral Blue** | `#1B3A48` | Textos principais, títulos e botões contrastantes |
| **Neutral White**| `#E6E6E6` | Fundos de cards, balões de depoimento e elementos neutros |

---

## 📂 Estrutura de Arquivos

```text
VetCare/
├── assets/
│   ├── icons/          # Ícones em formato SVG (email, whatsapp, telefone, pata, etc.)
│   └── img/            # Imagens e ilustrações SVG (depoimentos, estrutura, serviços, sobre, veterinários)
├── css/
│   ├── style.css       # Estilos globais, variáveis, reset, navbar e footer
│   ├── index.css       # Estilos da página inicial (hero, serviços, infra, depoimentos)
│   ├── sobre.css       # Estilos da página sobre nós
│   ├── servicos.css    # Estilos da listagem de serviços
│   ├── estrutura.css   # Estilos do carrossel e da galeria
│   ├── veterinarios.css# Estilos do corpo clínico e grade
│   ├── agendamento.css # Estilos do perfil dinâmico e formulário
│   └── contato.css     # Estilos da página de contato e mapa
├── pages/
│   ├── agendamento.html# Tela de agendamento e perfil do profissional
│   ├── contato.html    # Informações de contato e mapa
│   ├── estrutura.html  # Carrossel e galeria da clínica
│   ├── servicos.html   # Todos os serviços oferecidos
│   ├── sobre.html      # História, missão e valores
│   └── veterinarios.html# Lista dos profissionais da clínica
├── index.html          # Página principal da VetCare
└── README.md           # Documentação do projeto
```

---

## 🚀 Como Executar o Projeto

1. Clone o repositório ou faça o download dos arquivos:
   ```bash
   git clone https://github.com/anaclpsouza/VetCare.git
   ```
2. Abra a pasta do projeto no seu editor de preferência (ex.: VS Code).
3. Abra o arquivo `index.html` diretamente no seu navegador ou utilize uma extensão de servidor local como o **Live Server**.


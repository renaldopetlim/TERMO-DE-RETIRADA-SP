# 📄 Emissão de Termo de Retirada de Mercadoria

![HTML5](https://img.shields.io/badge/HTML5-%23E34F26.svg?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-%231572B6.svg?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-%23323330.svg?style=for-the-badge&logo=javascript&logoColor=%23F7DF1E)
![jsPDF](https://img.shields.io/badge/jsPDF-2.5.1-success?style=for-the-badge)
![LGPD](https://img.shields.io/badge/LGPD-Conforme-blue?style=for-the-badge)

Uma aplicação web ágil, segura e totalmente responsiva desenvolvida para a **Distribuidora São Paulo (CD Alça Viária)**. O sistema automatiza a criação de **Termos de Autorização para Retirada de Mercadoria**, vinculando representantes outorgados às Notas Fiscais Eletrônicas (NF-e) dos clientes para controle logístico e fiscal.

---

## ✨ Principais Recursos

- 📑 **Geração de PDF no Client-Side:** Processamento 100% local através da biblioteca [jsPDF](https://github.com/parallax/jsPDF). Os dados das NF-es e clientes não passam por servidores externos, garantindo privacidade e velocidade.
- 📐 **Algoritmo Auto-Fit de Paginação:** O PDF ajusta dinamicamente a escala dos elementos gráficos e fontes para garantir que o documento caiba perfeitamente em uma única página A4.
- ✍️ **Suporte à Assinatura Digital / Presencial:** Espaço reservado para validação jurídica via [gov.br](https://assinador.iti.br) (Lei nº 14.063/2020) ou registro de confirmação direta via WhatsApp.
- ⚠️ **Alerta para Vendas À Vista:** Exibição automática de modal informativo destacando o prazo máximo de **7 dias** para a retirada de pedidos pagos à vista.
- 🔒 **Conformidade com a LGPD:** Informes transparentes sobre o tratamento e armazenamento seguro dos dados (Art. 7º, II e V da Lei nº 13.709/2018).
- 🎭 **Validação e Máscaras em Tempo Real:**
  - Validação algorítmica de **CPF** e **CNPJ**.
  - Formatação de moeda em Real (**R$**).
  - Máscara para **Placa de Veículo** (padrão antigo e Mercosul) e telefone (**WhatsApp**).
  - Normalização automática para letras maiúsculas em campos de nomes.
- 🌓 **Suporte a Tema Escuro (Dark Mode):** Interface adaptável às preferências do sistema operacional ou navegador.

---

## 🛠️ Tecnologias Utilizadas

O projeto utiliza tecnologias web nativas (*Vanilla Web Development*), eliminando a necessidade de gerenciadores de pacotes ou servidores backend:

* **HTML5:** Marcação semântica e acessível.
* **CSS3:** Variáveis de estilo (*Custom Properties*), CSS Grid e Flexbox com design responsivo.
* **JavaScript (ES6+):** Manipulação de DOM, máscaras de entrada, validações matemáticas e fluxo de dados.
* **jsPDF (v2.5.1):** Engine para estruturação, estilização e renderização do PDF.

---

## 📁 Estrutura de Arquivos

```text
.
├── assets/
│   ├── logo.png         # Logo principal da empresa
│   └── logo-mini.ico    # Favicon da aplicação
├── index.html           # Interface principal da aplicação
├── style.css            # Estilização global, temas e layout
├── script.js           # Regras de negócio, validações e geração do PDF
└── README.md            # Documentação do projeto
```

---

## 📋 Fluxo de Utilização

1. **Preenchimento dos Dados:**
   - **Identificação:** Nº do Pedido e Data de Emissão.
   - **Cliente (Outorgante):** Razão Social/Nome, CPF/CNPJ, NF-e, Orçamento, Valor e Plano de Pagamento. *(Ao selecionar "A VISTA", o modal explicativo será exibido)*.
   - **Representante (Outorgado):** Nome do retirante, CPF, Cód. RCA e Placa do Veículo.
   - **Retirada:** Data, Horário e Local/Doca.
   - **WhatsApp (Opcional):** Dados de confirmação.

2. **Validação & Emissão:**
   - Clique em **"Gerar PDF"**. O sistema fará a checagem dos campos obrigatórios e da validade dos documentos.
   - O download do documento `Termo_Retirada_Pedido_[NUMERO].pdf` é iniciado automaticamente.

3. **Assinatura & Entrega:**
   - O documento gerado pode ser enviado para a assinatura digital do titular via [gov.br](https://assinador.iti.br) ou assinado presencialmente pela equipe de expedição no ato da entrega.

---

## 👨‍💻 Desenvolvedor

Desenvolvido por **Renaldo Petlim**.

[![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](https://github.com/renaldopetlim)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/renaldopetlim/)
[![Instagram](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/renaldopetlim/)
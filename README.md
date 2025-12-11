# 🎟️ Gerador de Rifas e Capas Otimizado para A4

Uma solução **client-side** leve e portátil, desenvolvida inteiramente com **HTML, CSS e JavaScript puro (Vanilla JS)**.

Este projeto foca na **eficiência de impressão**, gerando:
1.  **Talões de Rifa** com canhoto picotado e numeração automática.
2.  **Capas personalizáveis** com upload de imagem.

Ambos os layouts são rigorosamente formatados para caber **4 unidades por página A4**, prontos para impressão direta de qualquer navegador, sem a necessidade de um servidor web.

---

### ✨ Funcionalidades Principais

| Recurso | Descrição | Detalhes Técnicos |
| :--- | :--- | :--- |
| **Geração de Rifas** | Cria talões com numeração sequencial automática e canhoto picotado para contato do comprador. | 4 talões por página A4 (`height: 67.5mm`). Canhoto separado por `border-right: 1px dotted`. |
| **Geração de Capas** | Cria capas de rifa com espaço para nome, valor e data do sorteio. | 4 capas por página A4. Permite upload de imagem local (convertida para Base64). |
| **Interface Unificada** | A versão principal (`index.html`) consolida as funcionalidades de rifa e capa em uma única página. | Usa classes no `<body>` (`.printing-rifa`, `.printing-capa`) para controlar a visibilidade das seções na tela e na impressão. |
| **Otimização de Impressão** | Utiliza CSS `@media print` para garantir layout perfeito no formato A4, com margens mínimas. | Define `@page { size: A4 portrait; margin: 8mm; }` e esconde o formulário (`.no-print`) durante a impressão. |

---

### 🚀 Como Utilizar

O projeto é *self-contained* e não requer nenhuma configuração ou servidor web.

1.  **Baixar ou Clonar**: Clone este repositório para o seu computador.
2.  **Abrir no Navegador**: Clique duas vezes no arquivo principal (`src/index.html`) para abri-lo.
3.  **Preencher e Imprimir**: Insira os dados da rifa ou capa e clique no botão de impressão.

#### **Configurações Essenciais de Impressão:**

Ao abrir o diálogo de impressão do navegador (`Ctrl+P` ou `Cmd+P`), garanta que as seguintes configurações estejam aplicadas:

* **Orientação:** Retrato (Portrait)
* **Margens:** Mínimas ou Padrão.
* **Opções:** **DESATIVE** a impressão de **"Cabeçalhos e Rodapés"** (Headers and Footers) do navegador.

---

### 📂 Estrutura do Repositório

src/
├── index.html
├── rifa.html
└── capa.html
---

### 🤝 Contribuição

Sinta-se à vontade para abrir **Issues** para reportar bugs ou sugerir novas funcionalidades, ou enviar **Pull Requests** com melhorias.

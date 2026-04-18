# Sistema ERP Premium v4

Um sistema de gestão empresarial (ERP) completo e moderno, desenvolvido em um único arquivo HTML com design premium e funcionalidades avançadas.

## 📋 Visão Geral

Este ERP é uma solução completa para pequenas e médias empresas, oferecendo gestão financeira, controle de pedidos, vendas, despesas, clientes e precificação, tudo em uma interface intuitiva e responsiva.

## ✨ Funcionalidades Principais

### 📊 Painel Financeiro (Dashboard)
- Receitas, despesas e lucro líquido em tempo real
- DRE (Demonstrativo de Resultado do Exercício) automático
- Cálculo de ponto de equilíbrio
- Gráficos de evolução mensal
- Sparklines de tendências
- Comparativo mês atual vs. anterior

### 📦 Central de Pedidos
- Cadastro e acompanhamento de pedidos
- Status: Produção, Pronto, Entregue, Cancelado
- Alertas de prazo (atrasado, atenção, urgente)
- Controle de pagamentos parciais
- Integração com WhatsApp para cobrança
- Cálculo automático de CMV (Custo de Mercadoria Vendida)

### 🛒 Vendas
- Registro de vendas de pronta entrega
- Histórico completo de vendas
- Relatórios exportáveis em Excel

### 💸 Despesas
- Lançamento de despesas operacionais
- Despesas fixas recorrentes (automatizadas)
- Categorização de gastos
- Controle por período

### 👥 Clientes
- Cadastro completo de clientes
- Histórico de pedidos por cliente
- Faturamento e inadimplência
- Modal de detalhes com estatísticas

### 🏷️ Precificação & Ficha Técnica
- Almoxarifado de insumos
- Montagem de fichas técnicas de produtos
- Cálculo automático de custos de produção
- Sugestão de preço de venda com margem personalizável

### 🤖 Inteligência Artificial
- Diagnóstico rápido da saúde financeira
- Score de saúde do negócio (0-100%)
- Insights automáticos sobre operação
- Alertas de logística e inadimplência
- Recomendações personalizadas

### ⚙️ Configurações
- Personalização de cores (tema)
- Upload de logo da empresa
- Gestão de usuários (Firebase Auth)
- Backup e restauração de dados (JSON)

## 🎨 Design & UX

- **Design Premium**: Interface moderna com gradientes, sombras suaves e glassmorphism
- **Totalmente Responsivo**: Funciona em desktop, tablet e mobile
- **Dark Mode Ready**: Estrutura preparada para temas escuros
- **Animações Fluidas**: Transições suaves e feedback visual
- **Toast Notifications**: Sistema de notificações elegante
- **Modais Interativos**: Confirmações e diálogos bem desenhados

## 🔧 Tecnologias Utilizadas

| Tecnologia | Finalidade |
|------------|------------|
| HTML5 | Estrutura semântica |
| CSS3 Moderno | Estilização com variáveis CSS, Grid, Flexbox |
| JavaScript (Vanilla) | Lógica e interatividade |
| Firebase (v10.8.1) | Autenticação e Firestore (banco de dados) |
| Chart.js (4.4.1) | Gráficos e visualizações |
| Lucide Icons | Ícones modernos e leves |
| Google Fonts (Outfit) | Tipografia elegante |

## 🚀 Como Usar

### Opção 1: Abrir Localmente
```bash
# Basta abrir o arquivo no navegador
open erp_premium_v4.html
```

### Opção 2: Servidor Local (Recomendado para Firebase)
```bash
# Com Python
python -m http.server 8000

# Com Node.js (npx)
npx serve

# Acesse no navegador
http://localhost:8000/erp_premium_v4.html
```

### Configuração do Firebase

Para habilitar autenticação e banco de dados na nuvem:

1. Crie um projeto no [Firebase Console](https://console.firebase.google.com/)
2. Ative **Authentication** (Email/Senha)
3. Ative **Firestore Database**
4. Copie as credenciais do projeto
5. No código, substitua a configuração do Firebase:

```javascript
const firebaseConfig = {
    apiKey: "SUA_API_KEY",
    authDomain: "SEU_PROJETO.firebaseapp.com",
    projectId: "SEU_PROJECT_ID",
    storageBucket: "SEU_BUCKET",
    messagingSenderId: "SEU_SENDER_ID",
    appId: "SEU_APP_ID"
};
```

## 📁 Estrutura do Projeto

```
/workspace
└── erp_premium_v4.html    # Arquivo único com todo o sistema
```

### Seções do Código

| Linhas | Seção | Descrição |
|--------|-------|-----------|
| 1-200+ | `<style>` | Todo o CSS do sistema |
| 200-400+ | HTML Structure | Layout, modais, formulários |
| 400-2282 | `<script>` | Toda a lógica JavaScript |

## 📊 Módulos do Sistema

| Módulo | Descrição |
|--------|-----------|
| **Dashboard** | Visão geral financeira com KPIs |
| **Performance** | Métricas operacionais e rankings |
| **Pedidos** | Gestão completa do ciclo de pedidos |
| **Vendas** | Registro e histórico de vendas |
| **Despesas** | Controle de saídas financeiras |
| **Clientes** | CRM integrado |
| **Preços** | Ficha técnica e precificação |
| **I.A.** | Insights inteligentes |
| **Configurações** | Personalização do sistema |

## 🔐 Segurança

- Autenticação via Firebase Auth
- Apenas administradores podem criar novos usuários
- Dados armazenados na nuvem (Firestore)
- Sessões persistentes e seguras

## 📱 Responsividade

O sistema é totalmente responsivo e se adapta a:
- 🖥️ Desktop (1400px+)
- 💻 Laptop (900px - 1400px)
- 📱 Tablet (600px - 900px)
- 📲 Mobile (< 600px)

## 🎯 Recursos Avançados

### Sistema de Toast
Notificações elegantes com 4 tipos:
- ✅ Successo
- ❌ Erro
- ⚠️ Atenção
- ℹ️ Informação

### Wizard de Pedido
Fluxo guiado passo-a-passo para criação de pedidos:
1. Dados do cliente
2. Itens do pedido
3. Pagamento
4. Revisão final

### Lookup Inteligente de Clientes
Ao digitar o nome do cliente, o sistema:
- Busca clientes existentes
- Sugere cadastro de novo cliente
- Mostra telefone e histórico

### Cálculo Automático de Prazos
- Define data de entrega baseada em dias úteis
- Considera urgência do pedido
- Alertas automáticos de vencimento

## 📈 Métricas e KPIs Disponíveis

- Receita Bruta
- Despesas Totais
- Lucro Líquido
- Margem Bruta e Líquida
- CMV (Custo de Mercadoria Vendida)
- Ticket Médio
- Taxa de Atraso
- Ponto de Equilíbrio
- Score de Saúde Financeira

## 🔧 Personalização

### Cores do Tema
O sistema usa variáveis CSS para fácil personalização:

```css
:root {
    --primary: #926cba;      /* Cor principal */
    --secondary: #d3a4ed;    /* Cor secundária */
    --success: #10b981;      /* Sucesso/verde */
    --danger: #f43f5e;       /* Erro/vermelho */
    --warning: #f59e0b;      /* Atenção/laranja */
    --info: #3b82f6;         /* Informação/azul */
}
```

### Logo da Empresa
- Upload de logo personalizada nas configurações
- Exibição no header, login e loading screen
- Formato recomendado: PNG ou SVG

## 📝 Backup de Dados

O sistema permite:
- **Exportar**: Baixa todos os dados em formato JSON
- **Importar**: Restaura dados de um backup JSON

## 🐛 Solução de Problemas

### Dados não salvam?
- Verifique a conexão com a internet
- Confirme se o Firebase está configurado corretamente
- Abra o console do navegador (F12) para ver erros

### Login não funciona?
- Verifique se o usuário foi criado pelo administrador
- Confirme as credenciais do Firebase Auth
- Limpe o cache do navegador

### Gráficos não aparecem?
- Verifique se o Chart.js está carregando
- Confira se há dados registrados no período selecionado

## 📄 Licença

Este projeto é de uso exclusivo para clientes do sistema ERP Premium.

## 👨‍💻 Suporte

Para suporte técnico e dúvidas:
- Verifique a documentação acima
- Analise os logs no console do navegador
- Contate o administrador do sistema

---

**Desenvolvido com ❤️ para simplificar a gestão do seu negócio**

*Versão: 4.0 | Última atualização: 2024*

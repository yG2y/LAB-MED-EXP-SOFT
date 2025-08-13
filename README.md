# 📊 Lab Experimentação e Medição de Software - GitHub Data Collector

## 📝 Descrição

Este notebook realiza coleta automatizada de dados de repositórios populares do GitHub utilizando a API GraphQL, permitindo análises estatísticas sobre maturidade, atividade, linguagens de programação e colaboração em projetos de código aberto.

## 🚀 Como Executar no Google Colab

### **Passo 1: Baixar o Arquivo**

1. Acesse o repositório onde o notebook está hospedado
2. Clique no arquivo `.ipynb` 
3. Clique no botão **"Download"** ou **"Raw"** e salve o arquivo em seu computador
4. Alternativamente, use o botão **"Download ZIP"** do repositório

### **Passo 2: Abrir no Google Colab**

1. Acesse [Google Colab](https://colab.google)
2. Faça login com sua conta Google
3. Na tela inicial, clique em **"Upload"** ou **"Carregar"**
4. Selecione o arquivo `.ipynb` que você baixou
5. O notebook será carregado automaticamente

**Alternativa - Via Google Drive:**
1. Faça upload do arquivo para seu Google Drive
2. Clique com botão direito no arquivo
3. Selecione **"Abrir com" → "Google Colaboratory"**

### **Passo 3: Configurar Token do GitHub**

⚠️ **IMPORTANTE**: O arquivo foi commitado sem o token por questões de segurança.

#### **3.1 - Obter Token do GitHub**

1. Acesse [GitHub Settings → Developer settings → Personal access tokens](https://github.com/settings/tokens)
2. Clique em **"Generate new token (classic)"**
3. Defina um nome descritivo (ex: "Colab Data Collection")
4. Selecione os escopos necessários:
   - `public_repo` (para repositórios públicos)
   - `read:org` (opcional, para dados organizacionais)
5. Clique em **"Generate token"**
6. **COPIE O TOKEN** (ele só aparece uma vez!)

#### **3.2 - Inserir Token no Notebook**

1. Localize a célula **"2. CONFIGURAÇÃO DO TOKEN"**
2. Substitua `"seu_github_token_aqui"` pelo seu token:


### **Passo 4: Executar o Notebook**

1. **Execute célula por célula**: Clique no botão ▶️ ao lado de cada célula
2. **Execute tudo**: Menu **"Ambiente de execução" → "Executar tudo"**
3. **Atalho**: `Shift + Enter` para executar célula atual

### **Passo 5: Teste de Conectividade**

Execute a seção **"3. TESTE DE CONECTIVIDADE"** para verificar se o token está funcionando corretamente:

- ✅ **Token válido**: Exibirá seu nome de usuário
- ❌ **Erro**: Verifique se o token foi copiado corretamente

## 📋 Estrutura do Notebook

| Seção | Descrição |
|-------|-----------|
| 1. Setup Inicial | Instalação das bibliotecas necessárias |
| 2. Configuração do Token | Inserção do token de acesso do GitHub |
| 3. Teste de Conectividade | Validação das credenciais |
| 4. Coleta de Dados | Execução das consultas GraphQL |
| 5. Análise dos Dados | Processamento e cálculo de métricas |
| 6. Visualizações | Geração de gráficos e relatórios |
| 7. Exportação | Salvamento dos dados coletados |

## 🔧 Requisitos

- **Conta Google** (para acessar o Colab)
- **Token do GitHub** (gerado conforme instruções acima)
- **Conexão com internet** (para acessar APIs)

## 📊 Dados Coletados

O notebook coleta as seguintes métricas para cada repositório:

- **Informações básicas**: Nome, descrição, URL
- **Métricas de popularidade**: Stars, forks
- **Atividade**: Idade, última atualização
- **Desenvolvimento**: Issues, Pull Requests, releases
- **Tecnologia**: Linguagem primária, licença
- **Colaboração**: Índices de participação externa

## ⚠️ Limitações e Considerações

- **Rate Limiting**: A API do GitHub tem limites de requisições
- **Token Privado**: Nunca compartilhe seu token em repositórios públicos
- **Dados Dinâmicos**: Os resultados podem variar conforme mudanças nos repositórios

## 🔒 Segurança

- O token **NÃO** está incluído no código por segurança
- Mantenha seu token privado e seguro
- Revogue tokens não utilizados nas configurações do GitHub

## 📁 Arquivos Gerados

Após a execução, o notebook gera:

- **CSV**: Dados tabulares para análise
- **JSON**: Dados brutos coletados
- **Relatório**: Resumo estatístico em texto
- **Gráficos**: Visualizações dos dados

## 🆘 Solução de Problemas

| Problema | Solução |
|----------|---------|
| "Token inválido" | Verifique se copiou o token completo |
| "Rate limit exceeded" | Aguarde alguns minutos antes de executar novamente |
| "Erro de conexão" | Verifique sua conexão com internet |
| "Bibliotecas não encontradas" | Execute a primeira célula de instalação |

## 🤝 Contribuições

<table>
  <tr>
    <td align="center">
      <a href="https://github.com/yG2y" title="Perfil Guilherme G2">
        <img src="https://avatars.githubusercontent.com/u/89223673?v=4" width="100px;" alt="Foto do Guilherme G2 no GitHub"/><br>
        <sub>
          <b>Guilherme G2</b>
        </sub>
      </a>
    </td>
  </tr>
</table>

**Desenvolvido para o Lab de Experimentação e Medição de Software** 📚

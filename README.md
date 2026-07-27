# 🏍️ FROTA LUZ - Sistema de Gestão de Motoboys

### Farmácia Luz - Rede Inova Drogarias

Sistema interno para controle de gastos dos motoboys: combustível, manutenção, entregas e indicadores gerenciais.

---

## 📁 Arquivos do Projeto

| Arquivo | Descrição |
|---------|-----------|
| `index.html` | Aplicativo completo (página principal) |
| `manifest.json` | Configuração para instalar como app no celular |
| `sw.js` | Service Worker para funcionar offline |
| `icon-192.png` | Ícone do app (192x192) |
| `icon-512.png` | Ícone do app (512x512) |

---

## 🚀 COMO PUBLICAR NO GITHUB PAGES (Passo a Passo)

### PASSO 1 - Criar conta no GitHub (se não tiver)

1. Acesse **https://github.com**
2. Clique em **"Sign up"**
3. Preencha e-mail, senha e nome de usuário
4. Confirme o e-mail

---

### PASSO 2 - Criar um repositório novo

1. Já logado no GitHub, clique no botão **"+"** no canto superior direito
2. Clique em **"New repository"**
3. Em **"Repository name"** digite: `frota-luz`
4. Marque **"Public"**
5. **NÃO** marque "Add a README file" (os arquivos já estão prontos)
6. Clique em **"Create repository"**

---

### PASSO 3 - Enviar os arquivos

#### Opção A: Pelo próprio site do GitHub (mais fácil)

1. Na página do repositório recém-criado, clique em **"uploading an existing file"**
2. Arraste **TODOS os 5 arquivos** desta pasta para a área de upload:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icon-192.png`
   - `icon-512.png`
3. Embaixo, em "Commit changes", pode deixar como está
4. Clique no botão verde **"Commit changes"**

#### Opção B: Pelo Git no terminal (para quem já usa)

```bash
cd frota-luz
git init
git add .
git commit -m "FROTA LUZ - Sistema de Gestão de Motoboys"
git branch -M main
git remote add origin https://github.com/SEU_USUARIO/frota-luz.git
git push -u origin main
```

---

### PASSO 4 - Ativar o GitHub Pages

1. No repositório, clique em **"Settings"** (engrenagem no menu superior)
2. No menu lateral esquerdo, clique em **"Pages"**
3. Em **"Source"**, selecione **"Deploy from a branch"**
4. Em **"Branch"**, selecione **"main"** e a pasta **"/ (root)"**
5. Clique em **"Save"**
6. **Aguarde 1-2 minutos**
7. Atualize a página — vai aparecer o link do seu site:

```
https://SEU_USUARIO.github.io/frota-luz/
```

**Pronto! Esse é o link que funciona em qualquer computador e celular!** 🎉

---

## 📱 COMO INSTALAR NO CELULAR (como se fosse um App)

### No iPhone / Safari:
1. Abra o link no **Safari**
2. Toque no botão de **compartilhar** (quadrado com seta para cima)
3. Escolha **"Adicionar à Tela de Início"**
4. Toque em **"Adicionar"**

### No Android / Chrome:
1. Abra o link no **Chrome**
2. Toque nos **3 pontinhos** no canto superior direito
3. Escolha **"Adicionar à tela inicial"** ou **"Instalar aplicativo"**
4. Confirme

O app vai aparecer na tela do celular com o ícone vermelho "FL", como se fosse um aplicativo de verdade!

---

## 💾 Onde os dados ficam salvos?

Os dados ficam salvos no **localStorage do navegador**. Isso significa:

- ✅ Os dados persistem mesmo fechando e reabrindo o navegador
- ✅ Funciona offline depois do primeiro acesso
- ⚠️ Os dados são **por navegador** — se abrir no Chrome tem dados separados do Firefox
- ⚠️ Se limpar os dados do navegador, os registros serão apagados
- 💡 Use o mesmo navegador sempre para manter os dados

---

## ✏️ Como editar o sistema

O arquivo `index.html` contém todo o código. Abra com qualquer editor de texto:

- **Bloco de Notas** (Windows)
- **VS Code** (recomendado)
- **Notepad++**

### Coisas que você pode editar facilmente:

| O que editar | Onde encontrar no código |
|---|---|
| Cores do app | Procure por `--red:#dc2626` no início do CSS |
| Nome "FROTA LUZ" | Procure por `FROTA LUZ` no JavaScript |
| Nome "Farmácia Luz" | Procure por `Farmácia Luz` |
| Tipos de manutenção | Procure por `TIPOS_MANUT` |
| Dados de exemplo | Procure por `DEFAULT` (objeto com todos os dados iniciais) |

Depois de editar, salve o arquivo e envie novamente para o GitHub (faça um novo commit).

---

## 📊 Funcionalidades

- **Dashboard** — Gasto total, custo por entrega, custo por KM, consumo médio km/L
- **Motoboys** — Cadastro completo com moto, placa, telefone, CNH
- **Abastecimentos** — Registro com litros, valor, KM, posto
- **Manutenções** — Óleo, pneu, corrente, freio, revisão, elétrica
- **Entregas** — Quantidade diária e KM rodados por motoboy
- **Relatórios** — Ficha completa de cada motoboy com 8 indicadores
- **Ranking** — Classificação por eficiência (menor custo por entrega)

---

*Desenvolvido para uso interno da Farmácia Luz - Rede Inova Drogarias*

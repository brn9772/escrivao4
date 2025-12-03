# Escrivão - Transcritor de Reuniões com IA

## 🎯 O que é?

App web simples para transcrever e resumir áudios de reuniões usando IA (Whisper + LLaMA).

**Fluxo de uso:**
1. Grave suas reuniões no gravador de voz do celular
2. Faça upload do áudio no Escrivão
3. Adicione título e tags
4. Clique em "Gerar Resumo com IA"
5. Pronto! Você tem transcrição completa + resumo estruturado

## ✨ Features

- 📤 **Upload de áudio** (MP3, M4A, WAV, etc)
- 🏷️ **Sistema de tags** para organização
- 🔍 **Filtro por tags** na listagem
- 🤖 **Transcrição automática** com Whisper (Groq)
- 📝 **Resumo inteligente** com LLaMA:
  - Resumo geral
  - Principais pontos
  - Decisões tomadas
  - Ações e tarefas
- 💾 **Armazenamento local** (IndexedDB)
- 📱 **Funciona offline** após primeira carga
- 🔗 **Compartilhamento** via WhatsApp

## 🚀 Como usar

### 1. Configure a API (uma vez)
- Clique no ícone ⚙️
- Acesse https://console.groq.com
- Crie conta grátis
- Gere uma API key
- Cole no app

### 2. Adicione um áudio
- Clique em "+ Adicionar Áudio"
- Digite o título
- Adicione tags (opcional)
- Clique em "Selecionar Arquivo"
- Escolha o áudio do gravador
- Clique em "Salvar Reunião"

### 3. Gere o resumo
- Abra a reunião salva
- Clique em "Gerar Resumo com IA"
- Aguarde a transcrição (2-5min)
- Pronto! Você tem o resumo completo

## 📊 Capacidade

**Tamanhos recomendados:**
- ✅ Até 30min: ~10MB - Transcreve rápido (1-2min)
- ✅ 30min-1h: ~20MB - Divide em 2 partes
- ✅ 1h-2h: ~40MB - Divide em 3-4 partes
- ⚠️ Mais de 2h: Considere gravar em partes

**Formatos aceitos:**
- MP3, M4A, WAV, WEBM, OGG, AAC
- Qualquer formato de áudio do navegador

## 🔧 Tecnologias

- **Frontend**: HTML + CSS + JavaScript puro
- **Armazenamento**: IndexedDB (local no celular)
- **IA**: Groq API (100% grátis)
  - Whisper large-v3 (transcrição)
  - LLaMA 3.3 70B (resumo)
- **PWA**: Service Worker para funcionar offline

## ✅ Correções Aplicadas

### v3 - Simplificação
- Removida função de gravação ao vivo
- Foco 100% em upload de áudios
- Interface mais limpa e direta

### v2 - Divisão inteligente
- Áudios grandes divididos automaticamente
- Evita erro 413 "Request Too Large"
- Processa até 2h de áudio

### v1 - Base
- Upload de áudio
- Sistema de tags
- Transcrição e resumo com IA

## 💡 Dicas de uso

### Para melhores resultados:
- Grave em ambiente silencioso
- Use boa qualidade de áudio
- Fale claramente durante a reunião
- Adicione tags descritivas (ex: "loja07", "operações", "janeiro")

### Organização:
- Use tags consistentes (ex: sempre "operações" e não "operacao")
- Títulos descritivos facilitam busca
- Filtros por tag na tela inicial

### Performance:
- Áudios menores transcrevem mais rápido
- Para reuniões longas, grave em qualidade média
- Mantenha apenas reuniões importantes (libera espaço)

## 🐛 Troubleshooting

**"Arquivo muito grande"**
→ Comprima o áudio ou grave em qualidade menor

**"Erro ao gerar resumo"**
→ Verifique API key no ícone ⚙️

**"Transcrição vazia"**
→ Áudio pode estar corrompido ou muito ruído

**"Erro 413"**
→ Atualize para última versão (já corrigido)

## 📱 Instalação

1. Suba os arquivos no GitHub Pages
2. Acesse pelo navegador do celular
3. Configure a API key
4. Pronto para usar!

---

**Desenvolvido para Bruno @ Tintomax** 🎯  
**Versão 3.0 - Fevereiro 2025**

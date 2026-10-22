# Kroma Studio — versões

Instaladores do Kroma Studio e o arquivo que o programa consulta para saber se
há versão nova.

## Baixar

A versão mais recente está em [Releases](../../releases/latest).

O instalador é por usuário: não pede permissão de administrador e não mexe em
Arquivos de Programas. Quem já tem o Kroma Studio instalado não precisa baixar
daqui — o próprio programa avisa, baixa e instala sozinho.

## O que é o `kroma-studio.json`

É o manifesto que o programa lê:

```json
{
  "versao": "5.8.0",
  "url": "https://github.com/kromalab-studio/kroma-studio-releases/releases/download/v5.8.0/KromaStudio-5.8.0-Setup.exe",
  "tamanho": 220039844,
  "sha256": "44feb31cc25261aebdcf78f7f2fafd6e98ebc99ca543887b045dcf960ff32eaf",
  "obrigatoria": false,
  "notas": "o que mudou nesta versão"
}
```

O programa compara `versao` com a dele, baixa de `url` e só aceita o arquivo se
o `sha256` bater — é o que garante que o instalador chegou inteiro e é o nosso.

## Aviso do Windows

Os instaladores não têm assinatura digital paga, então o Windows pode mostrar
"Editor desconhecido" no primeiro download feito pelo navegador. Baixando pelo
próprio programa, pela atualização automática, esse aviso não aparece.

## Código

O código-fonte não está aqui: este repositório guarda só os instaladores.

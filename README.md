# BashGPT

The 'llm' script lets you ask questions to an LLM from your terminal.

The 'define' script uses the 'llm' script and lets you define words in the terminal 

`define artificial intelligence`

## Install

Link all scripts into a path directory.

## Config

Set environment variables
export BASHGPT_ENDPOINT='http://my-ollama-instance.net:11434/v1/chat/completions'
export BASHGPT_MODEL='qwen3:8b'

## Usage

Ask the LLM a question. 
```shell
llm "my question"
```

Optional `-p` flag to set a custom system prompt. Or system prompt can be changed directly in script.
```shell
llm -p "my custom prompt" "my question"
```

Optional `-l` flag stops current run from logging to chat history.
```shell
llm -l "my question"
```

Shows the definition of a word and tries to correct spelling.
```shell
define apokatastasis
```
## Requirements

- bash
- jq


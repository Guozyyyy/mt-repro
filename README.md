# mt-repro (anonymous review)

This repository provides a reproducibility package for Chinese→X low-resource MT instruction tuning.

## Contents
- instruction_dataset.zip (full package)
- 8 instruction files: refine_zh_{ug,ur,bo,he,bn,vi,id,fa}_instruction.json
- Example scripts (code_zh_ug/*.py)
- IWSLT/CCMatrix subset extraction tools

## Quick Start
unzip instruction_dataset.zip -d mt-repro
cd mt-repro

## Instruction data
Fields: id, src->tgt, instruction, input, output, score

## Running scripts
python code_zh_ug/self_instruct_zh_ug.py
python code_zh_ug/refine_zh_ug_input.py
python code_zh_ug/refine_zh_ug_instruction.py

## Environment
Python 3.9+. Common deps: torch, transformers, datasets, peft, accelerate, sentencepiece.

Prepared for double-blind review; avoid adding identifying information.


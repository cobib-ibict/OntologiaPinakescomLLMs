# Ontologia Pinakes

Este repositório contém os artefatos do projeto de geração da **Ontologia Pinakes**, via LLMs do Ibict, para representação de recursos bibliográficos

## 📄 Conteúdo do repositório

- `EspecificacaoDeRequisitos.docx`  
  Documento com 59 Questões de Competência (QCs), quadros conceituais e alinhamentos que serviram como base para a construção da ontologia.

- `Prompt_OntologiaPinakes_viaLLMs.txt`  
  Prompt detalhado elaborado para orientar modelos de linguagem de grande escala (LLMs) na geração automática da ontologia.

- `OntologiaPinakes_*.owl`  
  Arquivos RDF/XML gerados automaticamente pelos LLMs (ex: GPT-4o, Claude, Gemini) e manualmente no Protégé, representando a Ontologia Pinakes conforme as especificações.

## 🧩 Metodologia resumida

A ontologia foi gerada automaticamente a partir das especificações textuais, utilizando LLMs submetidos a um prompt que exigia:
- Classes em português sem acentos, propriedades camelCase, anotações `rdfs:label`, `rdfs:comment`, `rdfs:isDefinedBy` em pt-BR.
- Hierarquia e cardinalidades alinhadas ao LRM e PRESSoo, instâncias exemplificativas, e cadeias relacionais como `Biblioteca → Endereco → Localidade → UF → Regiao → Pais`.
- Saída em RDF/XML UTF-8, válida e importável no Protégé.

## 🔍 Como visualizar

Para explorar as ontologias geradas:
1. Abra os arquivos `.owl` no [Protégé](https://protege.stanford.edu/).
2. Navegue pelas classes, propriedades e instâncias geradas.
3. Compare as Ontologias geradas pelos LLMs com a OntologiaPinakes_Protege.owlgerada manualmente
4. Execute consultas SPARQL ou use as visualizações hierárquicas para explorar os modelos.

## 📝 Licença

Este projeto é distribuído sob a licença [Creative Commons CC BY 4.0](https://creativecommons.org/licenses/by/4.0/).

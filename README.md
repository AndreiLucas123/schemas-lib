# schemas-lib

**schemas-lib** é uma biblioteca Node.js inspirada no **Zod**, desenvolvida para validação de esquemas e tipagem estática em TypeScript. Assim como o Zod, **schemas-lib** oferece uma interface intuitiva e expressiva para definir e validar estruturas de dados, proporcionando uma experiência de desenvolvimento robusta e confiável.

## Características Principais

- Validação Simples e Clara: Defina esquemas de validação de forma fácil e compreensível.
- Integração Total com TypeScript: Aproveite a tipagem estática para garantir a segurança dos tipos em tempo de compilação.

## Diferenças com outras libs

A principal diferença está no reuso de **schemas** definidos para manter uma boa performance e clareza nas declarações, **schemas-lib** tem melhor escalabilidade em relação a performance de validação e da leitura do TypeScript, sem sacrificar muito DX

O **schemas-lib** gera a tipagem do objeto em uma propriedade do **meta**, `meta.jsType`aonde possue um Type do TypeScript

## Changelog

### [0.1.9] - 2024-08-08

Removed

- `deepEq` and `fast-deep-equal` dependency (May cause break changes)

### [0.1.7] - 2024-08-02

Added

Added `schema.errors({})`

Changed

Because of removal of `__DEV__`, jsType is always included on the meta

Removed

Removed support do `__DEV__` and `__SERVER__` variables, to make more easy to use **schemas-lib** in an existing project
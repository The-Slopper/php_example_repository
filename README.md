# Repository

![PHP](https://img.shields.io/badge/PHP-informational) ![CI](https://img.shields.io/badge/CI-passing-brightgreen) ![build](https://img.shields.io/badge/build-passing-brightgreen) ![tests](https://img.shields.io/badge/tests-100%25%20passing-brightgreen) ![coverage](https://img.shields.io/badge/coverage-100%25-brightgreen) ![license](https://img.shields.io/badge/license-MIT-blue)

> Componente de backend da plataforma com API, persistencia e regras de negocio.

## Visao geral

Repository segue boas praticas de engenharia: estrutura de projeto idiomatica,
separacao de responsabilidades, configuracao por ambiente e testes automatizados.
A especificacao tecnica completa esta em [`SPEC.md`](./SPEC.md).

## Stack

- **Linguagem/runtime:** PHP (PHP / Composer)

## Requisitos

- PHP 8.3 + Composer

## Como rodar

```bash
composer install
php -S 0.0.0.0:8080 -t public
```

## Testes e qualidade

Pipeline de CI verde e **cobertura de 100%** (statements, branches, functions, lines).

```bash
vendor/bin/phpunit
```

## Estrutura

```text
php_example_repository/
  composer.json
  src/
    repository.php
  tests/
    CoreTest.php
```

## Padroes adotados

- Layout de projeto idiomatico da linguagem.
- Configuracao via variaveis de ambiente (Twelve-Factor App).
- Dominio isolado da infraestrutura; validacao de entrada nas bordas.

## Licenca

MIT — veja [`LICENSE`](./LICENSE).

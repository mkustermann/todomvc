# todomvc

A Jaspr implementation of todomvc, written in Dart and compilable to either JavaScript or WebAssembly.

## Setup

Install [dart](https://dart.dev/get-dart).

Install Jaspr: `dart pub global activate jaspr_cli`.

## Running the project

Run your project using `jaspr serve`.

The development server will be available on `http://localhost:8080`.

## Building the project

Build your project using either:
- Generate JavaScript via: `jaspr build -O4 --extra-js-compiler-option=--no-minify`
- Generate WebAssembly via: `jaspr build -O4 --experimental-wasm --extra-wasm-compiler-option=--no-strip-wasm`

NOTE: The `--extra-{js,wasm}-compiler-option` are available with: https://github.com/schultek/jaspr/pull/397

The output will be located inside the `build/jaspr/` directory.

# Implementação de Grafo com Lista de Adjacências

## Notas do professor

Aqui segue um  [arquivo .h](https://github.com/eduardolfalcao/edii/blob/master/src/grafos/grafolistaadjexercicio.h)
com a assinatura das funções que eu gostaria que vocês implementassem. Aqui segue o arquivo de testes: [testGrafoListaAdj.cpp](https://github.com/eduardolfalcao/edii/blob/master/tests/testGrafoListaAdj.cpp)
## Dependências

- Gtest - 1.10.0-3 : Google Test -
  C++ testing utility based on the xUnit framework (like JUnit)

## instalar as dependências

Ubuntu ou outros derivados do Debian:

```shell
sudo apt install libgtest-dev 
```

Arch linux ou Derivados:

```shell
sudo pacman -S gtest
```
Caso você meu companheiro, companheira não tenha instalado
o kit básico de desenvolvimento,
também instale o **cmake**, **git**.

Ubuntu ou outros derivados do Debian:
```shell
sudo apt install build-essential git cmake 
```

Arch linux ou Derivados:

```shell
sudo pacman -S git base-devel cmake
```

### informações importatantes

A versão do compilador de C++ usada deve ser maior ou igual a versão **4.8.1**
uma vez que é utilizado C++11 nesse projeto, já o cmake foi configurado para aceitar
versões muito antigas de nó mínimo **2.8.12**, então tenha em mente que:

- sua versão do GCC deve ser maior ou igual __4.8.1__
- sua versão do cmake deve ser maior ou igual __2.8.12__

Para descobrir a sua versão atual do GCC digite no terminial:

```shell
gcc --version # deve ser maior que 4.8
```

Para descobrir a versão atual do cmake digite no terminal:

```shell
cmake --version # deve ser maior que 2.8.12
```

## Como testar no linux

```shell
mkdir build
cd build
cmake ..
make 
./runUnitTests
```

# Opengl and glfw project template

Para compilar no MSVC basta abrir o projeto na ide e compilar o executavel opengl_class

# Compilação

## Linux

1. Instale as biliotecas de desenvolvimento da sua distribuição da wayland e da x11
2. Na raiz do projeto crie a pasta build e entre nela
```bash
mkdir build && cd build

```
3. Crie os arquivos de compilação dentro da pasta build
```bash
cmake ..

```
4. Compile com a toolchain de escolha, por padrão é a do gnu com make
```bash
make -j12

```

## Clion
1. abra o projeto com a ide
2. clique no botão de run ou de compilação 

## MSVC
1. tenha as ferramentas de cmake instaladas na IDE

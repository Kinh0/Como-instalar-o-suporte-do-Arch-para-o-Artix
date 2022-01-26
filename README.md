<h1> Como instalar o suporte do Arch Linux para Artix Linux </h1>
> Status: Finished

### Para instalar o suporte do arch para o artix é muito simples e sem nenhum tipo de dor de cabeça, apenas faça o que for pedido abaixo:

#### Primeiramente instale o suporte apenas digite em seu terminal desta maneira: ``` > sudo pacman -S artix-archlinux-support ```

#### Segundamente use o seu editor de texto preferido como nano, neovim, vim, emacs e etc. use-os para modificar o repositorio localizado em /etc/pacman.conf desta maneira: ``` > sudo nvim /etc/pacman.conf ```

#### depois de ter aberto o arquivo vai aparecer algo parecido com isso: ![image](https://user-images.githubusercontent.com/91798869/151192608-4e836c0f-c4ab-44e7-9dce-d88380897a31.png)

#### Primeiro descomente a linha ```#ParallelDownloads = 5 ```
##### isso fará com que o seus downloads sejam mais rapido usando o pacman ⚠️

#### Após isto desça até a ultima linha do Código usando a cetinha do teclado ou o seu mouse.

#### E digite lá no final exatamente assim para não ter erro: ```
[community]
Include = /etc/pacman.d/mirrorlist-arch

[extra]
Include = /etc/pacman.d/mirrorlist-arch

[multilib]
Include = /etc/pacman.d/mirrorlist-arch ```

### Após este passo salve as mudanças com :wq no vim/nvim e ctrl+x no nano
#### em seguida ainda no seu terminal rode um ``` sudo pacman -Syu ``` para atualizar.

## Com tudo isso feito dessa exata maneira você ja pode desfrutar de sua nova maneira de Download.

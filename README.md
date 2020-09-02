# Configurações do ambiente

## Instalar Windows Subsystem Linux (WSL 1)

1. Abra o PowerShell em modo administrador e execute o seguinte comando:
```
Enable-WindowsOptionalFeature -Online -FeatureName Microsoft-Windows-Subsystem-Linux
```

2. Caso solicitado, reinicie o computador

## Instalar Ubuntu for Windows

1. Abra a Microsoft Store e pesquise por Ubuntu, selecione a versão padrão e baixe
2. Um prompt do Ubuntu aparecerá e irá te pedir para criar um username e password. Entre com as informações
3. Para atualizar a versão do Ubuntu:
    ```
    sudo apt-get update
    sudo apt-get upgrade
    ``` 

## Instalar o Firacode
1. A Firacode é uma fonte com ligatura e sua última versão pode ser encontrada [aqui](https://github.com/tonsky/FiraCode/releases).
2. As instruções para instalação podem ser encontradas [aqui](https://github.com/tonsky/FiraCode/wiki#installing-font).

## Instalar e configurar o Hyper

1. [Instalar o Hyper](https://hyper.is/)
2. Com o Hyper aberto, digitar ```ctrl + comma``` pra abrir as configurações
3. O arquivo editado configurado pode ser encontrado [aqui](https://github.com/anapaulalemos/environment-config/blob/master/hyper.js).

## Instalar o cURL e o Git
1. Para o cURL usamos 
```
sudo apt-get install curl
```

2. Para o Git:
```
    sudo apt-add-repository ppa:git-core/ppa
    sudo apt-get update
    sudo apt-get install git
```

## Instalar o Zsh e o Oh My Zsh

1. Para instalar o Zsh usamos 
``` 
sudo apt-get install zsh
```

2. Para instalar o [Oh My Zsh](https://github.com/ohmyzsh/ohmyzsh) usamos 
```
curl -L https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh | bash
```


## Instalar o Spaceship theme
1. Para o [Spaceship](https://github.com/pascaldevink/spaceship-zsh-theme) usamos o comando:
 ```
 curl -o - https://raw.githubusercontent.com/denysdovhan/spaceship-zsh-theme/master/install.zsh | zsh
 ```

## Instalar o plugin de autosugestão
1. Instalamos o [plugin](https://github.com/zsh-users/zsh-autosuggestions/blob/master/INSTALL.md) usando:
```
git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions
```

## Configurar o Oh My Zsh
1. Rodar o comando `vim ~/.zshrc` no hyper
2. Substituir pelo arquivo .zshrc [aqui](https://github.com/anapaulalemos/environment-config/blob/master/.zshrc).
3. Importante lembrar de trocar os paths do arquivo para o correto (todos arquivos com '__ana.lemos__' no path)

## Configurar o bash
1. Rodar o comando `vim ~/.bashrc` no hyper
2. Substituir pelo arquivo .bashrc [aqui](https://github.com/anapaulalemos/environment-config/blob/master/.bashrc)

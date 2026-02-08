![ranma1](https://i.ibb.co/R4G0HzzL/ranma1.png)
![ranma2](https://i.ibb.co/k2vk7340/ranma2.png)
![ranma3](https://i.ibb.co/0pf6GSBr/ranma3.png)
![ranma4](https://i.ibb.co/Cs4Qnmhb/ranma4.png)
![ranma5](https://i.ibb.co/qLnCXFYq/ranma5.png)
![ranma6](https://i.ibb.co/6cVkXZWd/ranma6.png)
![ranma7](https://i.ibb.co/zWhd8RLM/ranma7.png)

# COMO INSTALAR O TEMA

## EXTENSÕES NECESSÁRIAS
Para instalar temas no Gnome, você precisa de algumas extensões que podem ser baixadas aqui: https://extensions.gnome.org/
- [Install Browser Extension](https://extensions.gnome.org/) - Permite instalar extensões através do seu navegador.
- [User Themes](https://extensions.gnome.org/extension/19/user-themes/) - Carrega temas do shell a partir do diretório do usuário (ou seja, via pastas do seu computador).
- Gnome Tweaks - Você precisa desta ferramenta para gerenciar temas. Instale-a através da loja da sua distro ou digite o seguinte no terminal: ```sudo apt install gnome-tweaks```
- [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) - Permite colocar uma imagem de fundo na tela de bloqueio.
- [Dash to Dock](https://extensions.gnome.org/extension/307/dash-to-dock/) - Permite personalizar a dock.

## INSTALANDO O TEMA
Instale todas as extensões necessárias acima.

Vá para a pasta “home” e pressione Ctrl + H para visualizar as pastas ocultas (ou marque a opção para visualizar pastas ocultas) e crie uma pasta chamada **.themes** e **.icons**.

Extraia o arquivo .zip do tema, copie a pasta extraída e cole-a em .themes.

Abra o Gnome Tweaks, vá para Aparência e, em “Aplicativos” e “Shell”, selecione **RanmaTheme**, depois pressione Alt + F2 para reiniciar o shell e o tema estará instalado.

### COMO ALTERAR A COR DO DOCK
Para alterar a cor do dock, abra Extensões, clique em “Configurações” em “Dash to Dock”, vá para “Aparência” e em “Personalizar a cor do dash” insira a cor #0fc0fc.

### COMO INSTALAR O PAPEL DE PAREDE
Instale a extensão [Lock Screen Background](https://extensions.gnome.org/extension/1476/unlock-dialog-background/) no site Gnome Extensions. Pressione a tecla super e abra o aplicativo Extensões. Em Lock Screen Background, clique em Configurações, selecione o papel de parede e pronto.
As imagens a serem usadas como papéis de parede estão na pasta “images”.

### COMO COLOCAR A LOGO NO TERMINAL (FAST FETCH)
Primeiro gere um arquivos de configuração usando o comando abaixo no terminal:
<br>
```fastfetch --gen-config```
<br>
(será gerado o arquivo config.jsonc no local /.config/fastfetch/config.jsonc)

Pegue uma imagem e transform em ASCII. Você pode usar o site abaixo para isso. Depois copie e cole num bloco de notas e salve como "logo.txt".
https://www.asciiart.eu/image-to-ascii

Edite a clase "logo" do arquivo "config.jsonc" que está no caminho "/home/user/.config/fastfetch/config.jsonc", colocando o caminho para seu logo.txt. Exemplo de como deve ficar abaixo:
```
{
  "$schema": "https://github.com/fastfetch-cli/fastfetch/raw/dev/doc/json_schema.json",
    "logo": {
        "type": "file",
        "source": "/home/user/.config/fastfetch/logo.txt",
        "height": 15,
        "width": 30,
        "padding": {
            "top": 5,
            "left": 3
        }
    },
```

Para abrir o terminal com a logo sempre sem precisar digitar o comando fastfetch cole o comando abaixo no arquivo ".bashrc" no caminho "/home/user".
<br>
```fastfetch --logo /home/user/.config/fastfetch/logo.txt```

### COMO FAZER APARECER NOTIFICAÇÕES PARA TESTE
Digite o comando abaixo no terminal e uma notifiação falsa irá aparecer.
<br>
```notify-send "Título" "Mensagem de Teste"```

### COMO TIRAR SCREENSHOT DE QUALQUER AREA (COMO LOCKSCREEN E TELA DO PRINT)
Digite o comando abaixo no terminal e um print será tirado dentro de 10 segundos:
<br>
```gnome-screenshot -d 10```

### THEME COLORS
blue = #0fc0fc
<br>
pink = #fe4eda
<br>
yellow = #F5C211
<br>
green = #32cd32
<br>
red = #e62020 or #d40000
<br>
purple = #663399
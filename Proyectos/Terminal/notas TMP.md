
## Nota de Distrotube

##
Emacs  tiene 

chord: indica que fue una serie de 



Evil mode
en Emacs Doom el modmo evil mode (que es habilitar los shortcuts de vim) empiezan con la barra de espaceadora, aka space bar, y se abrevia com `SPC`   
para abrir y navegar en los proyectos seria algo como:
`SPC p p`
esto significa presionar espacio y depues la tecla p dos veces
\



`SPC w v` : para dividir la pantall (crea una ventasna hacia la derecha) o corta la ventana de manera  vertical 

`SPC W` => muestra el buffer de opciones pa evil mode 

`v` la V que se le agrega a `SPC w v`,significa _evil-window-vsplit_ vsplit=> de "vertical split"


`SPC w s` : para hacer vertical split 

`SPC w c` cierra el buffer (ventana ) actual 

### Movimientos
Moverte a la izq9uierda de la ventana
ch

c-l -> moverte arriba

c-j-> moverte hacia arriba
c-k-> moverte hacia abajo de la ventana




To open the Neotree view:
`SPC o n`






###
tmux

Session windows and panes
1 windows es a una session
Cada session tiene `n` panes

existe algo prefix key
generalmente es 
`ctrl + b` 
ahroa nombrada` <p>`

prefix +p

`<p> + z`  (pantalla de un pane)
`<p> + ! `se mueve entre sesiones (pero en pantalla completa)

`<p> +  x` => kill current pane
`<p> + w `=> lista las sesiones activas de tmux

ver tmux cheatsheet

`
unbind y usar control + space
```
unbind C-b
set C-space send-prefix

bind 

```


```
set -g @plugin 'catppuccin/tmux'
```

update de bash
sourc ./tmux/tmux.conf

```bash
asignar un numero a un pane 1 en lugar de 0
set -g base-index 1
set -g pane-base-index 1
set-windw-option -g pane-base-index 1 
set-option -g renumber-windows on

```



```bash
### Abrir varios panes de un mismo directorio en una sesion
#open panes in current directory
bind '"' split-window -v -c "#{pane_current_path}"
bind % split-window -h -c "#{pane_current_path}"
```
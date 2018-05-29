# Plantuml Previewer Vim
Vim/NeoVim plugin for preview [PlantUML](http://plantuml.com/)

![image](https://user-images.githubusercontent.com/1709861/40650003-dcd75a76-6364-11e8-8cb1-40d710a0cc0a.png)

## Dependencies
* Java
* Graphviz (https://www.graphviz.org/download/)
  * brew install graphviz
  * apt-get install graphviz
* [open-browser.vim](https://github.com/tyru/open-browser.vim)
* [aklt/plantuml-syntax](https://github.com/aklt/plantuml-syntax) (vim syntax file for plantuml)

## Usage
1. Start editing plantuml file in Vim
2. Run `:PlantumlOpen` to open previewer webpage in browser
3. Saving plantuml file in Vim, then previewer webpage will refresh

### Commands

#### PlantumlOpen
Open previewer webpage in browser, and watch current buffer

#### PlantumlStop
Stop watch buffer

#### PlantumlSave {filepath} [{format}]
Export uml diagram to file path  
Available formats  
> png, svg, eps, pdf, vdx, xmi,
> scxml, html, txt, utxt, latex

Example:
```
:PlantumlSave diagram.png
:PlantumlSave diagram.svg
```

### Variables
```
g:plantuml_previewer#plantuml_jar_path
```
Custom plantuml.jar file path

## Related
* [vim-slumlord](https://github.com/scrooloose/vim-slumlord)
* [previm](https://github.com/kannokanno/previm)

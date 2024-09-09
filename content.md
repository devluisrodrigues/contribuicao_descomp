# Erros Comuns relatados

Essa sessão está destinada a relatar os erros comuns que podem ocorrer ao tentar realizar uma simulação no modelsim.

## Erro: the -novopt option is now deprecated and will be removed in a future release.

> **Observação:** A solução é a mesma para Windows e Linux.

<img src="./img/novopt/erroNovopt.jpeg" alt="Erro: the -novopt option is now deprecated and will be removed in a future release." style="max-width:500px; max-height:300px;" />

Esse é um dos erros mais comuns e sua solução é muito simples. Basta remover a flag `-novopt` do arquivo de compilação do modelsim. 

Para isso, feche a janela com o erro. Em seguida, na janela do Modelsim, na parte superior, acesso Simulation -> Simulation Settings

<img src = "./img/novopt/exemploModelSim.png" alt="Janela model sim" style="max-width:500px; max-height:300px;" />

A seguinte aba irá aparecer

<img src = "./img/novopt/flagnovopt.jpeg" alt="Janela model sim" style="max-width:500px; max-height:300px;" />

Localize a flag `-novopt`, igual a que está na imagem acima, e a remova (apague apenas a flag `-novopt` e não o resto do comando). Após isso, clique em Save e rode a simulação novamente.

## Erro: ModelSim executable not found in ...

> **Observação:** A solução é muito parecida para Windows e Linux.

<img src="./img/Executable_not_found/erroModel.png" alt="Erro: Model" style="max-width:500px; max-height:300px;" />

Nesse caso, o erro ocorre porque o Modelsim não está conseguindo localizar o executável do Modelsim. Para resolver esse problema, é necessário adicionar o caminho do executável do Modelsim no EDA Tools Path.

Para isso, feche a janela com o erro, salve seu arquivo de simulação e, por fim, feche o ModelSim.

Em seguida, no Quartus, acesse Tools -> Options

<img src = "./img/Executable_not_found/quartusMenu.png" alt="Janela model sim" style="max-width:500px; max-height:300px;" />

A seguinte janela irá aparecer:

<img src = "./img/Executable_not_found/quartusOptions.png" alt="Janela model sim" style="max-width:500px; max-height:300px;" />

Selecione a aba EDA Tool Options

<img src = "./img/Executable_not_found/quartusEda.png" alt="Janela model sim" style="max-width:500px; max-height:300px;" />

Altere o caminho registrado no campo ModelSim-Altera. No caso de Linux, o caminho padrão é `/home/${USER}/IntelFPGA_lite/20.1/modelsim_ase/linuxaloem/`, enquanto no Windows é `C:/intelFPGA_lite/20.1/modelsim_ase/win32aloem/`. Após alterar o caminho, clique em OK e rode a simulação novamente.

Após realizar essa correção, abre o modelSim novamente e tente rodar a simulação.


## Erro: 


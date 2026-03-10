# Cenários de Teste

Documentação dos cenários de teste do desafio.

## Cadastro de Cursos
### Fluxo Principal
ID: CT01<br>
Cenário: Cadastrar curso com dados válidos<br>
Resultado esperado: O curso deve ser cadastrado com sucesso<br>

ID: CT02<br>
Cenário: Validar mensagem de sucesso após cadastro<br>
Resultado esperado: O sitema deve apresentar uma mensagem indicando o sucesso do cadastro<br>

ID: CT03<br>
Cenário: Verificar curso cadastrado<br>
Resultado esperado: O curso deve aparecer na lista<br>

### Validação de Campos
ID: CT04<br>
Cenário: Campos vazios<br>
Resultado esperado: O sistema deve exibir um erro de validação<br>

ID: CT05<br>
Cenário: Campos preenchidos com espaços<br>
Resultado esperado: O sistema deve impedir o cadastro<br>

ID: CT06<br>
Cenário: Campos preenchidos com tamanho mínimo<br>
Resultado esperado: Se dentro de uma regra, o sistema deve aceitar o cadastro<br>

ID: CT07<br>
Cenário: Campos preenchidos com tamanho máximo<br>
Resultado esperado: Se dentro de uma regra, o sistema deve impedir ou limitar a entrada de caracteres<br>

### Teste de Integridade
ID: CT08<br>
Cenário: Cadastro duplicado de curso<br>
Resultado esperado: O sistema deve tratar conforme a regra definida para o projeto<br>

ID: CT09<br>
Cenário: Cadastro com caracteres especiais<br>
Resultado esperado: O sistema deve tratar conforme a regra definida para o projeto<br>

ID: CT10<br>
Cenário: Cadastro de números em campos de nome<br>
Resultado esperado: O sistema deve tratar conforme a regra definida para o projeto<br>

### Outros Casos
ID: CT11<br>
Cenário: Campos com espaços antes e/ou depois<br>
Resultado esperado: O sistema deve remover ou realizar validação<br>

ID: CT12<br>
Cenário: Caracteres com acentuação<br>
Resultado esperado: O sistema deve aceitar<br>

ID: CT13<br>
Cenário: Campos com emojis ou caracteres não comuns<br>
Resultado esperado: O sistena deve tratar conforme a regra definida para o projeto<br>


## Listagem de Cursos
### Fluxo Principal
ID: CT14<br>
Cenário: Visualizar cursos<br>
Resultado esperado: Os cursos cadastrados devem ser visualizados<br>

ID: CT15<br>
Cenário: Atualização de lista após cadastro<br>
Resultado esperado: O novo curso deve ser apresentado na lista<br>

### Comportamentos
ID: CT16<br>
Cenário: Lista vazia<br>
Resultado esperado: O sistema deve apresentar algo indicando ausência de cursos cadastrados<br>

ID: CT17<br>
Cenário: Quantidade de cursos<br>
Resultado esperado: A lista deve continuar crescendo ou ser separada em páginas<br>

ID: CT18<br>
Cenário: Atualizar página<br>
Resultado esperado: Os cursos cadastrados devem continuar sendo apresentados, mantendo seus dados preservados<br>

### Teste de Usabilidade
ID: CT19<br>
Cenário: Verificar Informações<br>
Resultado esperado: As informações dos cursos listados devem ser claras<br>

ID: CT20<br>
Cenário: Alinhamento e organização<br>
Resultado esperado: A interface deve seguir um padrão previamente definido<br>


## Exclusão de Cursos
### Fluxo Principal
ID: CT21<br>
Cenário: Excluir curso existente<br>
Resultado esperado: O curso deve ser removido da lista<br>

ID: CT22<br>
Cenário: Confirmar exclusão<br>
Resultado esperado: O sistema deve confirmar a decisão de exclusão<br>

ID: CT23<br>
Cenário: Validar mensagem de sucesso após exclusão<br>
Resultado esperado: O sitema deve apresentar uma mensagem indicando o sucesso de exclusão do curso<br>

### Fluxo Alternativo
ID: CT24<br>
Cenário: Cancelar exclusão<br>
Resultado esperado: O curso deve permanecer na lista<br>

### Outros Casos
ID: CT25<br>
Cenário: Excluir último curso da lista<br>
Resultado esperado: O sistema deve apresentar algo indicando ausência de cursos cadastrados<br>

## Navegação entre Telas
ID: CT26<br>
Cenário: Alternar entre as telas "Cadastrar Curso" e "Listar Cursos"<br>
Resultado esperado: A navegação deve funcionar corretamente<br>

ID: CT27<br>
Cenário: Atualizar página na tela de cadastro de curso<br>
Resultado esperado: O formulário deve continuar totalmente funcional<br>

## Teste de UI
ID: CT28<br>
Cenário: Alinhamento de campos do formulário<br>
Resultado esperado: Os campos devem estar alinhados<br>

ID: CT29<br>
Cenário: Alinhamento da lista<br>
Resultado esperado: As colunas que apresentam os cursos devem estar organizadas<br>

ID: CT30<br>
Cenário: Espaçamento entre campos<br>
Resultado esperado: O espaçamento entre os campos deve ser consistente<br>

ID: CT31<br>
Cenário: Cor do botão de cadastro<br>
Resultado esperado: O botão deve indicar a ação principal de confirmação cadastro<br>

ID: CT32<br>
Cenário: Botão de exclusão<br>
Resultado esperado: O botão deve indicar a ação de exclusão<br>

ID: CT33<br>
Cenário: Estado hover dos botões<br>
Resultado esperado: Os botões devem ter um retorno visual ao passar o mouse<br>

ID: CT34<br>
Cenário: Mensagem de erro<br>
Resultado esperado: A mensagem deve ser clara e bem visível<br>

ID: CT35<br>
Cenário: Abrir página em outra aba<br>
Resultado esperado: Os dados devem permanecer consistentes<br>

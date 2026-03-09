# Cenários de Teste

Documentação dos cenários de teste do desafio.

## Cadastro de Cursos
### Fluxo Principal
ID: CT01
Cenário: Cadastrar curso com dados válidos
Resultado esperado: O curso deve ser cadastrado com sucesso

ID: CT02
Cenário: Validar mensagem de sucesso após cadastro
Resultado esperado: O sitema deve apresentar uma mensagem indicando o sucesso do cadastro

ID: CT03
Cenário: Verificar curso cadastrado
Resultado esperado: O curso deve aparecer na lista

### Validação de Campos
ID: CT04
Cenário: Campos vazios
Resultado esperado: O sistema deve exibir um erro de validação

ID: CT05
Cenário: Campos preenchidos com espaços
Resultado esperado: O sistema deve impedir o cadastro

ID: CT06
Cenário: Campos preenchidos com tamanho mínimo
Resultado esperado: Se dentro de uma regra, o sistema deve aceitar o cadastro

ID: CT07
Cenário: Campos preenchidos com tamanho máximo
Resultado esperado: Se dentro de uma regra, o sistema deve impedir ou limitar a entrada de caracteres

### Teste de Integridade
ID: CT08
Cenário: Cadastro duplicado de curso
Resultado esperado: O sistema deve tratar conforme a regra definida para o projeto

ID: CT09
Cenário: Cadastro com caracteres especiais
Resultado esperado: O sistema deve tratar conforme a regra definida para o projeto

ID: CT10
Cenário: Cadastro de números em campos de nome
Resultado esperado: O sistema deve tratar conforme a regra definida para o projeto

### Outros Casos
ID: CT11
Cenário: Campos com espaços antes e/ou depois
Resultado esperado: O sistema deve remover ou realizar validação

ID: CT12
Cenário: Caracteres com acentuação
Resultado esperado: O sistema deve aceitar

ID: CT13
Cenário: Campos com emojis ou caracteres não comuns
Resultado esperado: O sistena deve tratar conforme a regra definida para o projeto

## Listagem de Cursos
### Fluxo Principal
ID: CT14
Cenário: Visualizar cursos
Resultado esperado: Os cursos cadastrados devem ser visualizados

ID: CT15
Cenário: Atualização de lista após cadastro
Resultado esperado: O novo curso deve ser apresentado na lista

### Comportamentos
ID: CT16
Cenário: Lista vazia
Resultado esperado: O sistema deve apresentar algo indicando ausência de cursos cadastrados

ID: CT17
Cenário: Quantidade de cursos
Resultado esperado: A lista deve continuar crescendo ou ser separada em páginas

ID: CT18
Cenário: Atualizar página
Resultado esperado: Os cursos cadastrados devem continuar sendo apresentados, mantendo seus dados preservados

### Teste de Usabilidade
ID: CT19
Cenário: Verificar Informações
Resultado esperado: As informações dos cursos listados devem ser claras

ID: CT20
Cenário: Alinhamento e organização
Resultado esperado: A interface deve seguir um padrão previamente definido

## Exclusão de Cursos
### Fluxo Principal
ID: CT21
Cenário: Excluir curso existente
Resultado esperado: O curso deve ser removido da lista

ID: CT22
Cenário: Confirmar exclusão
Resultado esperado: O sistema deve confirmar a decisão de exclusão

### Fluxo Alternativo
ID: CT23
Cenário: Cancelar exclusão
Resultado esperado: O curso deve permanecer na lista

### Outros Casos
ID: CT24
Cenário: Excluir último curso da lista
Resultado esperado: O sistema deve apresentar algo indicando ausência de cursos cadastrados

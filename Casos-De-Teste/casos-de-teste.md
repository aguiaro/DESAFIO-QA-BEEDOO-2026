# Casos de Teste

Documentação dos casos de teste do desafio.

## Feature: Cadastro de Cursos
Como usuário do sistema<br>
Quero cadastrar cursos<br>
Para que eles possam ser visualizados posteriormente<br>

Cenário: CT01 - Cadastrar curso com dados válidos<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele preenche os campos obrigatórios com dados válidos<br>
E confirma o cadastro<br>
Então o curso deve ser cadastrado com sucesso<br>

Cenério: CT02 - Validar mensagem de sucesso após cadastro<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele cadastra um curso com dados válidos<br>
Então o sistema deve exibir uma mensagem de sucesso informando que o curso foi cadastrado<br>

Cenário: CT03 - Verificar curso cadastrado na lista<br>
Dado que um curso foi cadastrado com sucesso<br>
Quando o usuário acessa a lista de cursos<br>
Então o curso cadastrado deve aparecer na listagem<br>

Cenário: CT04 - Tentar cadastrar curso com campos vazios<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele tenta cadastrar um curso sem preencher os campos obrigatórios<br>
Então o sistema deve exibir uma mensagem de erro de validação<br>

Cenário: CT05 - Tentar cadastrar curso com campos preenchidos apenas com espaços<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele preenche os campos apenas com espaços em branco<br>
E tenta salvar o cadastro<br>
Então o sistema deve impedir o cadastro do curso<br>

Cenário: CT06 - Cadastrar curso com tamanho mínimo permitido<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele preenche o campo nome com o tamanho mínimo permitido<br>
E confirma o cadastro<br>
Então o sistema deve permitir o cadastro do curso<br>

Cenário: CT07 - Cadastrar curso com tamanho máximo permitido<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele preenche o campo nome com o tamanho máximo permitido<br>
Então o sistema deve impedir ou limitar a entrada de caracteres conforme a regra definida<br>

Cenário: CT08 - Tentar cadastrar curso duplicado<br>
Dado que já existe um curso cadastrado com determinado nome<br>
Quando o usuário tenta cadastrar um novo curso com o mesmo nome<br>
Então o sistema deve tratar a duplicidade conforme a regra definida pelo projeto<br>

Cenário: CT09 - Cadastrar curso com caracteres especiais<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele insere caracteres especiais no campo de nome do curso<br>
E tenta realizar o cadastro<br>
Então o sistema deve tratar os caracteres conforme a regra definida pelo projeto<br>

Cenário: CT10 - Inserir números no campo de nome do curso<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele insere números no campo de nome<br>
E tenta realizar o cadastro<br>
Então o sistema deve tratar a entrada conforme a regra definida pelo projeto<br>

Cenário: CT11 - Cadastrar curso com espaços antes ou depois do nome<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele insere um nome com espaços antes ou depois do texto<br>
E confirma o cadastro<br>
Então o sistema deve remover os espaços extras ou realizar validação<br>

Cenário: CT12 - Cadastrar curso com caracteres acentuados<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele insere um nome com caracteres acentuados<br>
E confirma o cadastro<br>
Então o sistema deve permitir o cadastro do curso<br>

Cenário: CT13 - Cadastrar curso com emojis ou caracteres não comuns<br>
Dado que o usuário está na tela de cadastro de cursos<br>
Quando ele insere emojis ou caracteres não convencionais<br>
E tenta realizar o cadastro<br>
Então o sistema deve tratar a entrada conforme a regra definida pelo projeto<br>

## Feature: Listagem de Cursos
Como usuário do sistema<br>
Quero visualizar os cursos cadastrados<br>
Para consultar as informações disponíveis<br>

Cenário: CT14 - Visualizar cursos cadastrados<br>
Dado que existem cursos cadastrados no sistema<br>
Quando o usuário acessa a lista de cursos<br>
Então os cursos cadastrados devem ser exibidos<br>

Cenário: CT15 - Atualização da lista após novo cadastro<br>
Dado que o usuário cadastra um novo curso<br>
Quando ele acessa ou atualiza a lista de cursos<br>
Então o novo curso deve aparecer na listagem<br>

Cenário: CT16 - Visualizar lista quando não existem cursos cadastrados<br>
Dado que não existem cursos cadastrados<br>
Quando o usuário acessa a lista de cursos<br>
Então o sistema deve exibir uma mensagem indicando que não há cursos cadastrados<br>

Cenário: CT17 - Listagem com grande quantidade de cursos<br>
Dado que existem muitos cursos cadastrados<br>
Quando o usuário acessa a lista de cursos<br>
Então o sistema deve suportar o crescimento da lista ou aplicar paginação<br>

Cenário: CT18 - Atualizar página mantendo os cursos cadastrados<br>
Dado que existem cursos cadastrados no sistema<br>
Quando o usuário atualiza a página<br>
Então os cursos cadastrados devem continuar sendo exibidos<br>

Cenário: CT19 - Verificar clareza das informações dos cursos<br>
Dado que o usuário acessa a lista de cursos<br>
Quando os cursos são exibidos na tela<br>
Então as informações apresentadas devem ser claras e compreensíveis<br>

Cenário: CT20 - Verificar alinhamento e organização da interface<br>
Dado que o usuário acessa a lista de cursos<br>
Quando os cursos são exibidos<br>
Então a interface deve seguir o padrão visual definido<br>

## Feature: Exclusão de Cursos
Como usuário do sistema<br>
Quero excluir cursos cadastrados<br>
Para remover informações que não são mais necessárias<br>

Cenário: CT21 - Excluir curso existente<br>
Dado que existe um curso cadastrado<br>
Quando o usuário seleciona a opção de excluir o curso<br>
Então o curso deve ser removido da lista<br>

Cenário: CT22 - Confirmar exclusão de curso<br>
Dado que o usuário solicita a exclusão de um curso<br>
Quando o sistema solicita confirmação<br>
E o usuário confirma a exclusão<br>
Então o curso deve ser removido do sistema<br>

Cenário: CT23 - Validar mensagem de sucesso após exclusão<br>
Dado que o usuário está na tela listar cursos<br>
Quando ele seleciona a opção de excluir o curso<br>
E confirma a exclusão<br>
Então o sistema deve exibir uma mensagem de sucesso informando que o curso foi excluído<br>

Cenário: CT24 - Cancelar exclusão de curso<br>
Dado que o usuário solicita a exclusão de um curso<br>
Quando o sistema solicita confirmação<br>
E o usuário cancela a exclusão<br>
Então o curso deve permanecer na lista<br>

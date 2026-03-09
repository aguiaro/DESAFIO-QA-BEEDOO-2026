# Casos de Teste

Documentação dos casos de teste do desafio.

## Feature: Cadastro de Cursos
Como usuário do sistema
Quero cadastrar cursos
Para que eles possam ser visualizados posteriormente

Cenário: CT01 - Cadastrar curso com dados válidos
Dado que o usuário está na tela de cadastro de cursos
Quando ele preenche os campos obrigatórios com dados válidos
E confirma o cadastro
Então o curso deve ser cadastrado com sucesso

Cenério: CT02 - Validar mensagem de sucesso após cadastro
Dado que o usuário está na tela de cadastro de cursos
Quando ele cadastra um curso com dados válidos
Então o sistema deve exibir uma mensagem de sucesso informando que o curso foi cadastrado

Cenário: CT03 - Verificar curso cadastrado na lista
Dado que um curso foi cadastrado com sucesso
Quando o usuário acessa a lista de cursos
Então o curso cadastrado deve aparecer na listagem

Cenário: CT04 - Tentar cadastrar curso com campos vazios
Dado que o usuário está na tela de cadastro de cursos
Quando ele tenta cadastrar um curso sem preencher os campos obrigatórios
Então o sistema deve exibir uma mensagem de erro de validação

Cenário: CT05 - Tentar cadastrar curso com campos preenchidos apenas com espaços
Dado que o usuário está na tela de cadastro de cursos
Quando ele preenche os campos apenas com espaços em branco
E tenta salvar o cadastro
Então o sistema deve impedir o cadastro do curso

Cenário: CT06 - Cadastrar curso com tamanho mínimo permitido
Dado que o usuário está na tela de cadastro de cursos
Quando ele preenche o campo nome com o tamanho mínimo permitido
E confirma o cadastro
Então o sistema deve permitir o cadastro do curso

Cenário: CT07 - Cadastrar curso com tamanho máximo permitido
Dado que o usuário está na tela de cadastro de cursos
Quando ele preenche o campo nome com o tamanho máximo permitido
Então o sistema deve impedir ou limitar a entrada de caracteres conforme a regra definida

Cenário: CT08 - Tentar cadastrar curso duplicado
Dado que já existe um curso cadastrado com determinado nome
Quando o usuário tenta cadastrar um novo curso com o mesmo nome
Então o sistema deve tratar a duplicidade conforme a regra definida pelo projeto

Cenário: CT09 - Cadastrar curso com caracteres especiais
Dado que o usuário está na tela de cadastro de cursos
Quando ele insere caracteres especiais no campo de nome do curso
E tenta realizar o cadastro
Então o sistema deve tratar os caracteres conforme a regra definida pelo projeto

Cenário: CT10 - Inserir números no campo de nome do curso
Dado que o usuário está na tela de cadastro de cursos
Quando ele insere números no campo de nome
E tenta realizar o cadastro
Então o sistema deve tratar a entrada conforme a regra definida pelo projeto

Cenário: CT11 - Cadastrar curso com espaços antes ou depois do nome
Dado que o usuário está na tela de cadastro de cursos
Quando ele insere um nome com espaços antes ou depois do texto
E confirma o cadastro
Então o sistema deve remover os espaços extras ou realizar validação

Cenário: CT12 - Cadastrar curso com caracteres acentuados
Dado que o usuário está na tela de cadastro de cursos
Quando ele insere um nome com caracteres acentuados
E confirma o cadastro
Então o sistema deve permitir o cadastro do curso

Cenário: CT13 - Cadastrar curso com emojis ou caracteres não comuns
Dado que o usuário está na tela de cadastro de cursos
Quando ele insere emojis ou caracteres não convencionais
E tenta realizar o cadastro
Então o sistema deve tratar a entrada conforme a regra definida pelo projeto

## Feature: Listagem de Cursos
Como usuário do sistema
Quero visualizar os cursos cadastrados
Para consultar as informações disponíveis

Cenário: CT14 - Visualizar cursos cadastrados
Dado que existem cursos cadastrados no sistema
Quando o usuário acessa a lista de cursos
Então os cursos cadastrados devem ser exibidos

Cenário: CT15 - Atualização da lista após novo cadastro
Dado que o usuário cadastra um novo curso
Quando ele acessa ou atualiza a lista de cursos
Então o novo curso deve aparecer na listagem

Cenário: CT16 - Visualizar lista quando não existem cursos cadastrados
Dado que não existem cursos cadastrados
Quando o usuário acessa a lista de cursos
Então o sistema deve exibir uma mensagem indicando que não há cursos cadastrados

Cenário: CT17 - Listagem com grande quantidade de cursos
Dado que existem muitos cursos cadastrados
Quando o usuário acessa a lista de cursos
Então o sistema deve suportar o crescimento da lista ou aplicar paginação

Cenário: CT18 - Atualizar página mantendo os cursos cadastrados
Dado que existem cursos cadastrados no sistema
Quando o usuário atualiza a página
Então os cursos cadastrados devem continuar sendo exibidos

Cenário: CT19 - Verificar clareza das informações dos cursos
Dado que o usuário acessa a lista de cursos
Quando os cursos são exibidos na tela
Então as informações apresentadas devem ser claras e compreensíveis

Cenário: CT20 - Verificar alinhamento e organização da interface
Dado que o usuário acessa a lista de cursos
Quando os cursos são exibidos
Então a interface deve seguir o padrão visual definido

## Feature: Exclusão de Cursos
Como usuário do sistema
Quero excluir cursos cadastrados
Para remover informações que não são mais necessárias

Cenário: CT21 - Excluir curso existente
Dado que existe um curso cadastrado
Quando o usuário seleciona a opção de excluir o curso
Então o curso deve ser removido da lista

Cenário: CT22 - Confirmar exclusão de curso
Dado que o usuário solicita a exclusão de um curso
Quando o sistema solicita confirmação
E o usuário confirma a exclusão
Então o curso deve ser removido do sistema

Cenário: CT23 - Cancelar exclusão de curso
Dado que o usuário solicita a exclusão de um curso
Quando o sistema solicita confirmação
E o usuário cancela a exclusão
Então o curso deve permanecer na lista

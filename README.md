# Solarium UI

Desenvolvido pela equipe Lua, o Solarium UI é um produto voltado para a fácil e rápida criação e publicação de aulas, usando mídias nos formatos de texto, imagem, vídeo e links externos.

# Requisitos implementados

Código | Funcionalidade                                                         | Situação      | Localização
-------|------------------------------------------------------------------------|---------------|--------------
RF0001 | Mostrar tela "Login"                                                   | CONCLUÍDO     | [App.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/App.js), linha 15 <br/> [cadastro.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Login/index.js), linha 107 <br/> [aulas.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Aulas/aulas.js), linhas 28 e 29 (função `redirectToLogin`) <br/> [editor.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Editor/editor.js), linhas 140 e 141 (função `redirectToLogin`)
RF0002 | Mostrar tela "Cadastro"                                                | CONCLUÍDO     | [App.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/App.js), linha 20 <br/> [index.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Login/index.js), linha 78
RF0003 | Mostrar tela de recuperação de senha                                   | CONCLUÍDO     | [App.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/App.js), linha 21 <br/> [index.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Login/index.js), linha 117
RF0004 | Mostrar tela de redefinição de senha                                   | CONCLUÍDO     | [App.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/App.js), linha 22 (acessada apenas via link enviado via email, após ação na recuperação de senha)
RF0005 | Mostrar tela "Disciplinas"                                             | NÃO INICIADO  | -
RF0006 | Mostrar tela de disciplina ativa                                       | NÃO INICIADO  | -
RF0007 | Mostrar tela “Aulas”                                                   | INICIADO      | [App.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/App.js), linha 17 <br/> [editor.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Editor/editor.js), linha 266 <br/> [index.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Login/index.js), linhas 61 e 62 (função `redirectToList`)
RF0008 | Logar fornecendo usuário e senha válidos                               | CONCLUÍDO     | [signin.js](https://github.com/jpedroarag/Solarium-API/blob/main/auth/signin.js), linhas 5-27
RF0009 | Cadastrar-se no sistema                                                | CONCLUÍDO     | [signup.js](https://github.com/jpedroarag/Solarium-API/blob/main/auth/signup.js), linhas 11-35
RF0010 | Recuperar senha fornecendo e-mail válido                               | CONCLUÍDO     | [authentication.js](https://github.com/jpedroarag/Solarium-API/blob/main/auth/authentication.js), linhas 38-77
RF0011 | Redefinir senha                                                        | CONCLUÍDO     | [authentication.js](https://github.com/jpedroarag/Solarium-API/blob/main/auth/authentication.js), linhas 79-117
RF0012 | Salvar aula como rascunho                                              | CONCLUÍDO     | API => [lessonCrud.js](https://github.com/jpedroarag/Solarium-API/blob/main/lessons/lessonCrud.js), linhas 31-50 <br/> Interface => [editor.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Editor/editor.js), linhas 95-132 (função `saveChanges`)
RF0013 | Editar rascunho de aula                                                | INICIADO      | API => [lessonCrud.js](https://github.com/jpedroarag/Solarium-API/blob/main/lessons/lessonCrud.js), linhas 61-75 <br/> Interface => [editor.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Editor/editor.js), linhas 95-132 (função `saveChanges`)
RF0014 | Excluir rascunho de aula                                               | CONCLUÍDO     | API => [lessonCrud.js](https://github.com/jpedroarag/Solarium-API/blob/main/lessons/lessonCrud.js), linhas 52-59 <br/> Interface => [aulas.js](https://github.com/jpedroarag/Solarium-UI/blob/main/src/Pages/Aulas/aulas.js) linhas 53-75 (função `removeElement`)
RF0015 | Publicar aula                                                          | NÃO INICIADO  | -
RF0016 | Editar aula publicada                                                  | NÃO INICIADO  | -
RF0017 | Excluir aula publicada                                                 | NÃO INICIADO  | -
RF0018 | Desfazer a última ação                                                 | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0019 | Refazer a última ação                                                  | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0020 | Inserir texto                                                          | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0021 | Formatar texto em negrito                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0022 | Formatar texto em itálico                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0023 | Formatar texto sublinhado                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0024 | Formatar texto tachado                                                 | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0025 | Alinhar à esquerda                                                     | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0026 | Alinhar à direita                                                      | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0027 | Alinhar ao centro                                                      | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0028 | Justificar                                                             | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0029 | Definir estilo de texto como “Parágrafo”                               | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0030 | Definir estilo de texto como “Título 1”                                | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0031 | Definir estilo de texto como “Título 2”                                | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0032 | Definir estilo de texto como “Título 3”                                | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0033 | Escolher o tamanho da fonte                                            | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0034 | Escolher a fonte                                                       | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0035 | Selecionar a cor da fonte                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0036 | Selecionar a cor de fundo                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0037 | Inserir imagem                                                         | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0038 | Inserir vídeo                                                          | INICIADO      | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0039 | Inserir link externo                                                   | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0040 | Tornar lista (numerada)                                                | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0041 | Tornar lista (marcadores)                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0042 | Tornar checklist                                                       | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0043 | Tornar citação                                                         | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0044 | Tornar bloco de citação                                                | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0045 | Inserir bloco de citação                                               | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0046 | Aumentar recuo                                                         | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0047 | Diminuir recuo                                                         | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0048 | Criar tabela                                                           | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0049 | Transformar em coluna de cabeçalho                                     | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0050 | Inserir coluna à esquerda                                              | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0051 | Inserir coluna à direita                                               | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0052 | Selecionar coluna                                                      | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0053 | Deletar coluna                                                         | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0054 | Unir a célula acima                                                    | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0055 | Unir a célula a direita                                                | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0056 | Unir a célula abaixo                                                   | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0057 | Unir a célula a esquerda                                               | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0058 | Dividir célula verticalmente                                           | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0059 | Dividir célula horizontalmente                                         | CONCLUÍDO     | Feito por plugin adicionado ao CKEditor. A configuração dos plugins se encontra em [ckeditor.js](https://www.github.com/jpedroarag/Solarium-UI/blob/main/ckeditor5-custom-build/src/ckeditor.js).
RF0060 | Criar tags personalizadas*                                             | SUSPENSO      | -
RF0061 | Filtrar conteúdo do Material de Apoio via tags*                        | SUSPENSO      | -
RF0062 | Estabelecer vínculo entre uma aula e um arquivo do Material de Apoio*  | SUSPENSO      | -
RF0063 | Remover vínculo entre uma aula e um arquivo do Material de Apoio*      | SUSPENSO      | -

# Detalhes sobre cliente e equipe

## Cliente

O cliente é o professor Wellington Wagner Ferreira Sarmento, do curso de Sistemas e Mídias Digitais da Universidade Federal do Ceará.

## Membros da equipe

Matrícula | Membro                                
----------|------------------------------------- 
474120    | Daniel Alves Furtado                  
472262    | Heloise Barreto Sá                    
494119    | João Pedro Aragão Felício             
472207    | João Victor Teixeira Cavalcante       
473850    | José Cleiton Carneiro Filho           

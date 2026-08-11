Casos de Teste: Fluxo de Recuperação de Senha 

Este repositório contém a documentação técnica que elaborei para validar o Fluxo de  "Esqueci minha Senha" e redefinição de credenciais de acesso.

pré-condição: Usuário cadastrado no sistema
passos:
1. clicar em "esqueci minha senha"
2. digitar e-mail cadastrado e clicar em enviar
3. abrir o e-mail e copiar o código de verificação e colar na pagina de recuperação de senha ou clicar no link de validação de Usuário pra confirmar sua identidade.
4. digitar a nova senha e preencher a confirmação de senha.
5. clicar em salvar.

resultado esperado: senha redefinida com sucesso, Usuário sendo redirecionado pra pagina de login.

tentativa com o e-mail não cadastrado
pré-condição: nenhuma
passos:
1.clicar em "esqueci minha senha"
2. O Usuário digitar o e-mail que não está cadastrado e clicar em enviar 

resultado esperado: O sistema deve enviar bloquear o envio e exibir a mensagem: "E-mail não encontrado" ou "Usuário inválido"

tentativa com senha fraca
pré-condição: O usuário já deve ter clicado no link de redefinir senha
passos:
1.No campo "nova senha" digitar ex:'123'
2.No campo confirme sua senha, digitar novamente '123'
3.clicar em salvar

resultado esperado: o sistema deve bloquear o envio e exibir a mensagem "a senha deve conter no mínimo 8 caracteres, incluindo letras e números"

senhas diferentes no preenchimento:
pré-condição: O usuário já deve ter clicado no link de redefinir senha
passos:
1. No campo "nova senha" digite ex:'123'
2. No campo "confirme a senha" digite ex:'321'
3. apertar no botão enviar

resultado esperado: o sistema deve bloquear o envio e exibir a mensagem "as senhas não coincidem".







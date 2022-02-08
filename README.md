# devsuperior-validation-and-security

Desafio BootCamp DEVSUPERIOR - Cap 03 - Validação e Segurança

Foram implementadas as funcionalidades necessárias para que os testes do projeto disponibilizado passem.

Neste sistema, somente as rotas de leitura (GET) de eventos e cidades são públicas (não precisa de login). 
Usuários CLIENT podem também inserir (POST) novos eventos. 
Os demais acessos são permitidos apenas a usuários ADMIN.

Validações de City:
- Nome não pode ser vazio

Validações de Event:
- Nome não pode ser vazio
- Data não pode ser passada
- Cidade não pode ser nula

Regras de autorização do ResourceServerConfig descritas em linguagem natural.
1) Os endpoints de login e do H2 devem ser públicos
2) Os endpoints GET para /cities e /events devem ser públicos
3) O endpoint POST de /events devem requerer login de ADMIN ou CLIENT
4) Todos demais endpoints devem requerer login de ADMIN

TDD - Test Driven Development
É um método de desenvolver software. Consiste em um desenvolvimento guiado pelos testes.

Princípios / vantagens:
- Foco nos requisitos
- Tende a melhorar o design do código, pois o código deverá ser testável
- Incrementos no projeto têm menos chance de quebrar a aplicação

Processo básico:
- Escreva o teste como esperado (naturalmente que ele ainda estará falhando)
- Implemente o código necessário para que o teste passe
- Refatore o código conforme necessidade

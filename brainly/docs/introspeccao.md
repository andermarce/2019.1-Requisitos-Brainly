# Introspecção

Introspecção é uma técnica muito rica e profunda para a elicitação de requisitos. Através desse método, o indivíduo que pretende levantar os requisitos faz observações e descrições do conteúdo (pensamentos, sentimentos) que decorrem da auto-reflexão sobre o serviço e, mediante a isso, é possível entender as propriedades que o sistema deve possuir para que atenda as necessidades do seu público.

As introspecções descritas abaixo, são divididas em três tópicos principais: contexto, necessidades do contexto e requisitos elicitados. Para contextualizar a introspecção, utilizou-se a ideia de um _storytelling_, em que há uma persona que  desempenha uma atividade na plataforma. Decorrente do contexto, foi feita uma auto-reflexão para elencar as necessidades técnicas, sociais e individuais da persona, o que em seguida decorre na elicitação dos requisitos.

## Introspecção 1 - Fluxo de perguntas e respostas

#### Rastreabilidade

|Papel | Data | Nome | Observação |
|--|--|--|--|
| Autor | 08/04/2019 | Welison Regis | Membro da equipe/Usuário |


#### Contexto

João, graduando em técnologo em análise e desenvolvimento de sistemas, é um estudante exemplar, sendo destaque em sua turma da faculdade. Cansado das atividades monótonas da faculdade, decidiu procurar uma plataforma que possibilitasse o acesso a diversas questões abertas de outros estudantes de forma que ele pudesse praticar o que estivesse aprendendo e, além disso, ajudar outra pessoa; depois de alguns minutos, João conheceu o Brainly.

Após criar sua conta no serviço, João, jovem astuto em programação, decidiu responder uma pergunta que solicitava ajuda na implementação de uma ordenação através do algoritmo _bubble sort_ utilizando a linguagem java. Em um primeiro momento, João escreveu uma solução que explicou o algoritmo, adicionando imagens que auxiliava na explicação da solução, porém, João não gostou do fato de não poder colocar o seu código bem formatado na resposta, e também por não possuir recurso de destaque para citações.

Finalizada a resposta, João decidiu compartilhar a questão para que seja possível que seus colegas de faculdade que estão estudando o mesmo assunto tenham acesso a explicação do algoritmo e, assim, facilitar o entendimento sobre o conteúdo.

#### Necessidades do Contexto
Este tópico indicará as necessidades acarretadas pelo contexto.

##### Necessidades Técnicas
*   Acesso a um dispositivo que tenha internet.
*   _Design_ intuitivo para usuários iniciantes utilizarem as ferramentas disponibilizadas sem dificuldade.

##### Necessidades Sociais
Para compartilhar o conhecimento gerado, João necessita de:

*   Compartilhamento das questões entre amigos e seguidores para disseminar conhecimento, seja em rede social ou outro mensageiro.
*   Possibilidade de comunicar e tirar dúvidas nas próprias questões.
*   Contactar aos amigos usuários da aplicação as atividades desempenhadas na plataforma.

##### Necessidades Individuais
Para discorrer uma resposta de qualidade, João necessita de:

*   Disposição de campo para escrever a resposta, campo este que possibilitará destacar a resposta (negrito, itálico, sublinhado) e aumentar fonte da letra.
*   Possibilitar o anexo de soluções de arquivos de tamanho razoável em quaisquer formatos.
*   Dispor de recursos de `highlight` para inserir citações e códigos fontes em questões de informática.
*   Ferramenta que facilite digitar expressões matemáticas, seja simbolos ou `LaTeX`.
*   Possibilitar consistência na ferramenta de texto entre as diversas plataformas.

#### Requisitos Elicitados

| Código | Requisito | Descrição | Prioridade |
| :----: | :-------: | :-------: | :--------: |
| INT1.1 | Compartilhar questão | O usuário pode compartilhar questões da plataforma  | - |
| INT1.2 | Comunicação aos seguidores | O _feed_ das contribuições de um usuáiro para a plataforma podem ser visualizadas por outros usuários da plataforma | - |
| INT1.3 | Comunicação na questão | É possível se comunicar e retirar dúvidas nos comentários da própria questão. | - |
| INT1.4 | Recursos textuais | O sistema deve fornecer recursos de escrita, como: negrito, itálico, sublinhado, diferentes tamanhos de texto | - |
| INT1.5 | Recursos de anexos | O sistema deve suportar diversos formatos de anexos que ocupem um espaço razoável | - |
| INT1.6 | Recurso de notações matematícas | O sistema deve facilitar a inserção de símbolos matemáticos, assim como textos em LaTeX | - |
| INT1.7 | Recursos de _hightlight_ | O sistema deve fornecer recurso de _hightlight_ (destaque) para certas informações, como citações | - |
| INT1.8 | Recursos de programação | O sistema deve possibilitar a inserção adequada de código-fonte | - |
| INT1.9 | Consistência ferramental | A ferramenta que possibilita respostas deve ser consistente entre as plataformas | - |

## Introspecção 2 - Moderação de perguntas e respostas

|Papel | Data | Nome | Observação |
|--|--|--|--|
| Autor | 09/04/2019 | Welison Regis | Membro da equipe/Usuário |

Lucas, moderador na plataforma Brainly, responde às demandas de denúncias e dúvidas de usuários no site. Em atividades cotidianas, depara-se com perguntas e respostas com brincadeiras, insultos, assédios ou outros problemas do gênero.

Concorrente a Lucas tem Guilherme, usuário que já não tem mais pontos e que decidiu obter a pontuação da forma mais rápida possível: digitando besteiras nas respostas das questões. Porém, Guilherme foi rapidamente denunciado por outros usuários, o que acarretou na exclusão de suas brincadeiras e em advertência ao usuário, aplicadas por Lucas, moderador da plataforma.


##### Necessidades Técnicas
*   Acesso a um dispositivo que tenha internet.
*   Consistência entre as múltimas versões (mobile, web) da plataforma;
*   Disponibilização das ferramentas de moderação entre as múltiplas versões da plataforma.

##### Necessidades Sociais
Para tratar ações como a de Guilherme, a plataforma necessita de:

*   Dispor recurso de denúncia a usuários fora das regras da plataforma;
*   Ter funcionários e voluntários que possam verificar a procedência das denúncias e aplicar as devidas punições.

##### Necessidades Individuais
Para moderar com qualidade, Lucas necessita de:

*   Treinamento por parte da administração para tratar as demandas do site.
*   Ferramenta que possibilite a exclusão do conteúdo indevido e que registre a penalidade ao perfil do usuário;
*   Ferramenta para bloquear, deletar ou banir o usuário da plataforma.
*   Macros com as mensagens padrões para moderação.

#### Requisitos Elicitados

| Código | Requisito | Descrição | Prioridade |
| :----: | :-------: | :-------: | :--------: |
| INT2.1 | Denúncia à irregularidade | O sistema deve oferecer um meio ao qual os usuários podem denunciar irregularidades em perguntas, respostas ou comentários | - |
| INT2.2 | Moderação multiplataforma | Deve ser possível ao moderador e à administração a gerência de conteúdos em qualquer que seja a plataforma de uso da aplicação | - |
| INT2.3 | Aperfeiçoamento da moderação | As ações dos moderadores devem ser pautadas por treinamentos e ensinamentos por parte da administração | - |
| INT2.4 | Macros de moderação | A administração deve dispor macros de moderação para facilitar a atuação na plataforma | - |
| INT2.5 | Ferramenta de exclusão de conteúdo | O sistema deve dispor aos moderados e à administração ferramentas que possibilitem a exclusão de conteúdos indevido | - |
| INT2.6 | Ferramenta de repressão intensiva | A plataforma deve dispor aos moderadores e à administração ferramentas para bloquear, deletar e banir péssimos usuários da plataforma | - |

## Introspecção 3 - Usuários com maior fluxo de perguntas

|Papel | Data | Nome | Observação |
|--|--|--|--|
| Autor | 09/04/2019 | André Pinto | Membro da equipe/Usuário |

Verônica, aluna do fundamental, estuda diariamente em casa, realizando exercícios e consequentemente surgem diversas duvidas que precisam de uma resposta razoavelmente rápida, pois não quer acumular matéria. Verônica conhece o Brainly e passa a colocar suas duvidas na plataforma, que em sua maioria são respondidas dentro de 10 minutos, porem as vezes encontra alguma resposta errada ou sem sentido que são posteriormente denunciada por outros usuários e apagadas por moderadores. Certo dia a turma Verônica sai com uma duvida da sala e a moca, ao chegar em casa, posta a pergunta na plataforma e compartilha em sua rede social predileta, o facebook, para ajudar seus colegas.

Por outro lado, Paulo, aluno do ensino médio, costuma esquecer de responder seus deveres de casa, lembrando apenas no ônibus indo para a escola. Em uma jornada para escola, Paulo, conhece o Brainly, cria sua conta utilizando o facebook e coloca uma duvida na plataforma, com ajuda de fotos para agilizar o processo, sendo respondida antes de chegar na escola e consequentemente realizando o dever no prazo.

##### Necessidades Técnicas
*   Acesso a um dispositivo que tenha internet;
*   Design intuitivo, bonito e de fácil manuseio;
*   Consistência entre as diferentes plataformas (mobile, web);
*   Disponibilizar ao usuário ferramentas para responder e perguntar.

##### Necessidades Sociais
Para melhor atender Verônica, a plataforma necessita de:

*   Existência de moderadores;
*   Possibilidade de exclusão de respostas irrelevantes;
*   Possibilidade de compartilhar pergunta/resposta em rede social.

Para melhor atender Paulo, a plataforma necessita de:

*   Possibilidade de entrar utilizando alguma rede social;

##### Necessidades Individuais
Para melhor atender Verônica, a plataforma necessita de:

*   Bom tempo médio de resposta;
*   Possibilidade de denunciar respostas .

Para melhor atender Paulo, a plataforma necessita de:

*   Possibilidade de entrar utilizando alguma rede social;
*   Rápida curva de aprendizagem;
*   Bom tempo médio de resposta;
*   Possibilidade de enviar fotos anexadas;
*   Economia de internet em dispositivos mobile;
*   Existência de uma versão mobile;

#### Requisitos Elicitados
Foi utilizado o MoSCoW para dar prioridade aos requisitos.

| Código | Requisito | Descrição | Prioridade |
| :----: | :-------: | :-------: | :--------: |
| INT3.1 | Existência de moderadores | O sistema deve possuir pessoas cuidando e analisando denuncias para evitar respostas irrelevantes | S |
| INT3.2 | Ferramentas para moderação | O sistema deve dar aos moderadores ferramentais para que eles possam atuar da melhor forma possível | S |
| INT3.3 | Consistência entre plataformas | O sistema deve oferecer a mesma experiência para usuários de diferentes plataformas | C |
| INT3.4 | Compartilhar em redes sociais | A plataforma deve oferecer ferramentas para que os usuários possam compartilhar as respostas nas redes sociais | C |
| INT3.5 | Logar com redes sociais | A plataforma deve oferecer um meio para que o usuário entre em sua conta a partir de redes sociais | C |
| INT3.6 | Bom tempo médio de respostas | A plataforma deve possuir membros ativos que ajudem a comunidade a crescer e respondam as perguntas de forma rápida e fácil | M |
| INT3.7 | Compartilhar em redes sociais | A plataforma deve oferecer ferramentas para que os usuários possam compartilhar as respostas nas redes sociais | C |
| INT3.8 | Denunciar resposta/conta | A plataforma deve oferecer ao usuário maneiras de denunciar algo que não condiz com as regras, facilitando e auxiliando moderadores | M |
| INT3.9 | Curva rápida de aprendizagem | A plataforma ter uma boa curva de aprendizagem, sem causar impacto aos novos usuários | M |
| INT3.10 | Anexo de imagens | A plataforma deve oferecer ferramentas para que os usuários possam compartilhar as perguntas/respostas com auxilio de imagens, facilitando o fluxo | S |
| INT3.11 | Versão mobile | O sistema deve possuir uma versão mobile de fácil acesso e com baixo consumo de bateria/dados | S |
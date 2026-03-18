# W-UAI Baja
### Wireless Unit for Acquisition & Integration

Boas vindas à interface de telemetria da equipe **Baja UFMG**!
Siga os passos abaixo para instalar o aplicativo e ver instruções de uso. Boas setagens!

## Instruções de Instalação
1. Faça o download do arquivo [`setup.exe`](https://baja-ufmg-2025.github.io/W-UAI-Distrib/setup.exe).
>[!TIP]
>O navegador possivelmente não reconhecerá o arquivo. Se necessário, clique com o botão direito no download e selecione "Manter".
2. Execute o arquivo.
>[!IMPORTANT]
>Se uma janela azul aparecer, indicando que o windows não confia no executável, clique em `Mais informações` e o botão de "Executar mesmo assim" aparecerá.
3. Siga os passos indicados e aceite a instalação na janela que aparecer. Os pré-requisitos, como os redistributáveis C++ e o .NET 8.0 serão instalados. Depois disso, a interface abrirá automaticamente. Tudo certo!
>[!NOTE]
>Toda vez que o aplicativo abrir, ele tentará se conectar à internet e vai procurar por atualizações. Dessa forma, você só precisa fazer o processo de instalação uma vez. 😉

## Instruções de Uso
- Para se beneficiar de uma experiência completa, é necessário o uso de uma **Estação de Telemetria** desenvolvida pelo Baja UFMG! Para se conectar a ela, basta utilizar um cabo USB ligado a qualquer porta do seu computador. Também é possível utilizar um módulo **USB-to-TTL**, comumente o ***PL2303 Prolific***, mas o seu uso necessita de conhecimento do circuito da estação, além de necessitar de um [driver específico para Windows](https://github.com/theAmberLion/Prolific).
- Ao abrir a interface, selecione a porta COM que equivale ao driver STMicroeletronics ou Prolific associado.
>[!TIP]
>Se não souber qual porta está ligada à Estação, basta desconectà-la e clicar em "Recarregar". A porta que sumir é a que você deve selecionar quando reconectar! PS: Também é possível abrir a interface antes de conectar a Estação, dessa forma você sabe quais portas já estão ligadas ao seu computador.
- Certifique-se de clicar no botão "Largada" para começar a ler e guardar os dados. Recomenda-se esperar o carro ser ligado, já que não terá nenhuma informação a ser lida caso contrário, o que pode causar um comportamento inesperado da inicialização dos gráficos.
- Para visualizar os dados depois do término da sessão, utilize a aba "Replay". Lá, você também pode exportar os dados daquela sessão nos formatos `.txt` e `.csv`, além de poder baixar a base de dados completa em `.db`.

## Descrição de Funcionalidades
### Enduro
- Dados visuais de velocidade, RPM e combustível.
- Descrição de voltas com tempo, velocidade média e pit stop.
- Janela de erros para fácil diagnóstico.
### Estrutura
- Dado visual de aceleração nos eixos x e y.
- Futuras versões apresentarão aceleração vertical e giro, e com a futura presença de extensômetros no carro, essa aba também será dedicada a eles.
### Pista
- Posição do carro em um mapa por satélite, com sua rota traçada com cores de acordo com a velocidade.
### Tempo Real
- Plot contínuo dos últimos 30 segundos de qualquer variável captada pela estação de telemetria.
### Replay
- Visualização dos dados que estão na base de dados por sessão. Caso se tenha dados de volta, calculados por GPS, é possível ver os dados de cada volta em uma seção dedicada.
### Botões
- **PIT-STOP** - Marcação manual de quando o carro parou de se mover ou retorna para o box. Apenas para de contabilizar o tempo de volta. Futuramente, será utilizado também para enviar ao piloto uma indicação de retorno ao box.
- **Largada/Chegada** - Serve para iniciar e fechar a sessão.
###
## Versões
| Número | Data | Descrição |
| --- | --- | --- |
| 1.0.2.0 | 18/03/2026 | Refatoração do painel de replay e tempo real, adição dos apelidos de sessão. |
| 1.0.1.4 | 12/03/2026 | Painel de estrutura melhorado, inicialização corrigida. |
| 1.0.0.2 | 09/03/2026 | Correções menores, padronização de nomes. |
| 1.0.0.0 | 09/03/2026 | Lançamento inicial, com funcionalidades completas de Enduro, Pista e Tempo Real. Aba de Estrutura incompleta. |


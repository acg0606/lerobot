# lerobot





ENTREGA

1. Dataset:
Gravação: Você precisa gravar um dataset de demonstrações de teleoperação. Isso envolve controlar o robô (SO-101, Koch, etc.) usando um dispositivo de teleoperação (outro braço robótico ou teclado) e registrar as ações e os dados dos sensores.
Número de Episódios: O tutorial sugere gravar pelo menos 50 episódios, com 10 episódios por local (se você estiver realizando uma tarefa em diferentes locais).
Upload para o Hugging Face Hub: Você deve fazer o upload do seu dataset para o Hugging Face Hub usando o comando huggingface-cli upload. O dataset será automaticamente marcado com "LeRobot" para facilitar a descoberta.
Nome do Repositório: O nome do repositório do dataset deve seguir o formato ${HF_USER}/nome-do-dataset.

2. Política Treinada (Modelo):
Treinamento: Você precisa treinar uma política (usando o script lerobot/scripts/train.py) para controlar o robô com base no seu dataset. O tutorial sugere usar a política "act" como ponto de partida.
Upload para o Hugging Face Hub: Você deve fazer o upload do checkpoint da política treinada para o Hugging Face Hub usando o comando huggingface-cli upload.

3. Demonstração (Vídeo de 1 Minuto):
Avaliação da Política: Você deve gravar um vídeo demonstrando a política treinada controlando o robô para realizar a tarefa.
Visualização: O vídeo deve mostrar o robô realizando a tarefa com sucesso.
Clareza: O vídeo deve ser claro e conciso, mostrando o que seu projeto faz e como ele funciona.

4. Documentação (Opcional, mas Recomendado):
Descrição do Projeto: Prepare uma breve descrição do seu projeto, explicando o problema que você está resolvendo e como sua solução funciona.
Instruções: Inclua instruções sobre como reproduzir seus resultados.


Resumindo:
Dataset no Hugging Face Hub
Modelo Treinado (Checkpoint) no Hugging Face Hub
Vídeo de Demonstração (menos de 1 minuto)

Recursos Importantes:

Comandos: Familiarize-se com os comandos lerobot.teleoperate, lerobot.record, lerobot/scripts/train.py e huggingface-cli.
Hugging Face Hub: Certifique-se de ter uma conta no Hugging Face Hub e de ter um token de acesso com permissão de escrita.

Documentação: Consulte a documentação oficial do LeRobot para obter informações detalhadas sobre a API e os comandos disponíveis.

Lembre-se de que o objetivo principal é demonstrar a capacidade de treinar uma política para controlar um robô real com base em dados de demonstração. Concentre-se em gravar um dataset de alta qualidade e treinar uma política que possa realizar a tarefa com sucesso.

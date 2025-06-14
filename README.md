# LeRobot Worldwide Hackathon
![image](https://github.com/user-attachments/assets/8a39b401-5670-45e7-8072-bb5e5935b9d5)

![image](https://github.com/user-attachments/assets/de501d45-9256-484f-992b-fa4118b8c2be)

LINKS
https://huggingface.co/LeRobot-worldwide-hackathon


https://huggingface.co/docs/lerobot/index
https://huggingface.co/datasets/LeRobot-worldwide-hackathon/Lerobot_dataset_V1
https://huggingface.co/datasets/LeRobot-worldwide-hackathon/datasets
https://huggingface.co/datasets/LeRobot-worldwide-hackathon/submissions
https://huggingface.co/datasets/LeRobot-worldwide-hackathon/laundrymasters-fold
https://huggingface.co/LeRobot-worldwide-hackathon/50000-MatchaMadness-new_arm
https://huggingface.co/docs/lerobot/en/getting_started_real_world_robot
https://huggingface.co/docs/lerobot/integrate_hardware

PDF
https://cdn-lfs-us-1.hf.co/repos/6a/6c/6a6cba86904a84ebd14b76fcdfd73322793b6e476811e98e2d9f0dc032803289/120d64a8a7ba1a8ee583814f0127476c03f219c372651298f4fcb5101c31069b?response-content-disposition=inline%3B+filename*%3DUTF-8%27%27Challenges.pdf%3B+filename%3D%22Challenges.pdf%22%3B&response-content-type=application%2Fpdf&Expires=1749923932&Policy=eyJTdGF0ZW1lbnQiOlt7IkNvbmRpdGlvbiI6eyJEYXRlTGVzc1RoYW4iOnsiQVdTOkVwb2NoVGltZSI6MTc0OTkyMzkzMn19LCJSZXNvdXJjZSI6Imh0dHBzOi8vY2RuLWxmcy11cy0xLmhmLmNvL3JlcG9zLzZhLzZjLzZhNmNiYTg2OTA0YTg0ZWJkMTRiNzZmY2RmZDczMzIyNzkzYjZlNDc2ODExZTk4ZTJkOWYwZGMwMzI4MDMyODkvMTIwZDY0YThhN2JhMWE4ZWU1ODM4MTRmMDEyNzQ3NmMwM2YyMTljMzcyNjUxMjk4ZjRmY2I1MTAxYzMxMDY5Yj9yZXNwb25zZS1jb250ZW50LWRpc3Bvc2l0aW9uPSomcmVzcG9uc2UtY29udGVudC10eXBlPSoifV19&Signature=u3lQzzMH6hV5oB7aQ%7E%7EjDyuYOQId%7EqrG4cgQtvvgc7pZVIRx3zslqzsL5l4nSBlya6vZIe2NVKlHypStEtqACIDwiXeEBn5PxB%7EeDoEE%7E2bNWLK5yo5IeDsXdETmSa%7Eb%7Ex717qI9uCr0Fu6zd2Rf0f0CwIdsF5nZ94VyMNGXkSuMzl7JtRW6x-u9rOdwgQd5sZBD-ku7ieE-wZsAWsQCknm6aZy2%7Ez-SljHaAsufeSmT%7EfZg3gcCdhlc5CXpi%7EilnuN6W%7EvvoAJx58-HoZ77ES35PD2UTHcm5iT26HaOiqUnRbHLptFcU9FM9SgLEXqmDrDsDh4Ol3QHSEymuUqbsA__&Key-Pair-Id=K24J24Z295AEI9

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

Passo 1: Gravação e Upload do Dataset (Simulador)
1.1 Configuração Inicial:
Login no Hugging Face Hub: (Mesmo passo)
huggingface-cli login --token ${HUGGINGFACE_TOKEN} --add-to-git-credential
Use code with caution.
Bash
Obtenha seu Nome de Usuário: (Mesmo passo)
HF_USER=$(huggingface-cli whoami | head -n 1)
echo $HF_USER
Use code with caution.
Bash

1.2 Gravação do Dataset (Simulador):
Execute o comando de gravação:
python -m lerobot.record \
    --robot.type=so101_follower \
    --robot.id=my_awesome_follower_arm \
    --display_data=true \
    --dataset.repo_id=${HF_USER}/so101_block_pickup \
    --dataset.num_episodes=2 \
    --dataset.single_task="Grab the black cube"
Use code with caution.
Bash

Importante: No simulador, você não precisa especificar as portas seriais (--robot.port e --teleop.port). O simulador lida com a comunicação internamente.
Você controlará o robô no simulador usando o teclado ou outro dispositivo de entrada.

1.3 Verificação do Upload: (Mesmo passo)
Acesse o link para verificar o upload:
https://huggingface.co/datasets/${HF_USER}/so101_block_pickup
Use code with caution.


Passo 2: Treinamento e Upload da Política (Simulador)

2.1 Treinamento da Política:

Execute o script de treinamento:
python lerobot/scripts/train.py \
  --dataset.repo_id=${HF_USER}/so101_block_pickup \
  --policy.type=act \
  --output_dir=outputs/train/act_so101_block_pickup \
  --job_name=act_so101_block_pickup \
  --policy.device=cuda \
  --wandb.enable=true
Use code with caution.
Bash
Os parâmetros são os mesmos do exemplo anterior.

2.2 Upload do Modelo Treinado: (Mesmo passo)
huggingface-cli upload ${HF_USER}/so101_block_pickup \
  outputs/train/act_so101_block_pickup/checkpoints/last/pretrained_model
Use code with caution.
Bash

2.3 Verificação do Upload: (Mesmo passo)
Acesse o link para verificar o upload:
https://huggingface.co/${HF_USER}/so101_block_pickup
Use code with caution.



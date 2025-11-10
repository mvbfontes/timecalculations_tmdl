# Cálculos de tempo no Power BI - código TMDL

Código para geração de calculation group no Power BI de "time intelligence" utilizando a aba "TMDL view".

Como utilizar:

1. Abra o Power BI Desktop: crie um novo relatório em branco ou abra um relatório existente;
2. No menu à esquerda, clique na aba "Model view";
3. Do lado direito na janela "Dados", clique na opção "Modelo";
4. Clique no nome "Modelo semântico" e na janela de "Propriedades" que irá se abrir, habilite a opção "Desestimular medidas implícitas" - esta etapa é necessária para habilitar a criação de calculation groups no modelo;
5. No menu à esquerda, clique em TMDL View — é a exibição de código do modelo;
6. É necessário ter uma dimensão de data no arquivo para o script funcionar corretamente. Caso seu relatório não tenha uma, utilize a dimensão de data que está neste repositório do Github (https://github.com/mvbfontes/dimensao_data_brasil);
7. Abra o arquivo "Script Time Intelligence.tmdl" (disponível neste repositório do Github) e clique no ícone de copiar no canto superior direito;
8. Volte ao Power BI e cole o código na TMDL View;
9. (Opcional) Confira se seu modelo possui uma dimensão de data e substitua todas as aparições no código pelo nome da sua tabela e sua coluna de data (o script original foi feito com uma tabela de data chamada "DimData" e coluna "Data");
<br><br>
<img width="645" height="322" alt="image" src="https://github.com/user-attachments/assets/7b0b5b52-1e30-4032-aaae-15c2138eef6a" />
<br><br>
10. Clique em "Aplicar" no canto superior esquerdo. Isso vai criar o calculation group "Time Intelligence" automaticamente; <br>
11. Depois, clique em "Atualizar agora" para carregar os dados; <br>
12. Confira a tabela "Time Intelligence" criada e atualizada na aba "Table view".



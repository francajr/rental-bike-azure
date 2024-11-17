<h3>Projeto de Machine Learning no Azure</h3>

**1. Configuração da Conta no Azure<br/>**
•	Criar uma conta no Microsoft Azure.<br/>
•	Criar um novo recurso Azure Machine Learning.<br/>
•	Ativar o Azure Machine Learning Studio.<br/>
•	Configurar permissões e cotas para o uso dos recursos de Machine Learning.<br/>

**2. Criar uma conta no Microsoft Azure. <br/>**
•	Criar um novo recurso Azure Machine Learning.<br/>
•	Ativar o Azure Machine Learning Studio.<br/>
•	Configurar permissões e cotas para o uso dos recursos de Machine Learning.<br/>

**3. Criação do Ambiente de Trabalho no Azure Machine Learning<br/>**
•	Criar uma nova instância em ML automatizado.<br/>
•	Configurar os recursos de acordo com a documentação.<br/>

**4. Desenvolvimento do Modelo Preditivo<br/>**
•	Carregar o conjunto de dados e realizar a preparação dos dados.<br/>
•	Escolher um algoritmo de aprendizado de máquina adequado.<br/>
•	Treinar o modelo no Azure Machine Learning Studio.<br/>
•	Avaliar a performance do modelo usando métricas apropriadas.<br/>

**5. Configuração dos Pontos de Extremidade<br/>**
•	Implantar os pontos de extremidade.<br/>
•	Salvar o arquivo de configuração JSON dos pontos de extremidade.<br/>

**6. Teste o serviço implantado<br/>**
•	Na página do endpoint em tempo real do predict-rentals , visualize a guia Teste . <br/>
•	No painel Dados de entrada para testar o ponto de extremidade , substitua o JSON do modelo pelos seguintes dados de entrada: <br/>

**7. Teste o serviço implantado<br/>**
•	Na página do endpoint em tempo real do predict-rentals, visualize a guia Teste .<br/>
•	No painel Dados de entrada para testar o ponto de extremidade, substitua o JSON do modelo pelos seguintes dados de entrada:<br/>
```
   {
  "input_data": {
    "columns": [
      "day",
      "mnth",
      "year",
      "season",
      "holiday",
      "weekday",
      "workingday",
      "weathersit",
      "temp",
      "atemp",
      "hum",
      "windspeed"
    ],
    "index": [0],
    "data": [[1,1,2022,2,0,1,1,2,0.3,0.3,0.3,0.3]]
  }
 }
```

•	Devendo retornar o valor igual ou semelhante a:<br/>

```
[
   352.3564674945718
 ]
```

**8. Limpar<br/>**
•	No Azure Machine Learning Studio , na guia Endpoints , selecione o endpoint predict-rentals . Em seguida, selecione Delete e confirme que deseja excluir o endpoint.<br/>
•	No portal do Azure , na página Grupos de recursos , selecione o grupo que deseja Excluir e selecione Excluir .<br/>

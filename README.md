# DIO-Microsoft-Azure-AI-Fundamentals
Para trabalhar no machine learn é essencial que você possua um workspace e esta é a tarefa inicial, criar o seu workspace para assim poder criar o seu trabalho automatizado.

Depois que nosso worlspace estiver pronto temos que entrar no ML studio para criar um "novo trabalho de ML automatizado", seguindo o passo a passo da documentação do Learning para melhor entendimento e para que tudo dê certo:
![01](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/a728e5c1-45fd-4684-8e1f-0ad45265c1e1)


## Vamos criar um aprendizado de maquina para a previsão de aluguel de bicicletas:
![02](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/e4251817-469d-41ea-99a8-9275ff431489)

O tipo de tarefa: regressão
o nome de ativo de dados: aluguel de bicicletas, com fonte de dados da WEB.
![03](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/0653807a-2b3b-442f-b0b0-cdc1775979c0)
![04](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/81fd030a-ddec-460f-991f-2a43431ca921)
![05](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/602a7ce8-f679-43aa-983c-6237d61330a9)

Adocumentação do Learning é bem didática e traz todos os valores e configurações para que o trabalho automatizado seja criado:


![07](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/ed29f470-78fd-417f-ba2b-e81a3b695eb7)
![08](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/804d6046-a206-4110-bdc5-5238991266c1)
![09](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/53eabfac-286d-48b1-bf91-e12b5aa62d3f)
![10](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/b99e1abd-dad5-4eb7-a30e-9be7c84031e7)
![11](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/6767d50a-1a53-40de-b50f-45b13c9b4b62)
![12](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/9b488264-697d-48cf-88be-d6d4481be99b)
![13](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/a1a2ce35-9088-4a57-9ff1-753d747dd4f5)
Chegando na opção "examinar" basta enviar o seu trabalho de treinamento:
![14](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/7ce847c0-a284-408d-afba-cc94c58298fe)

Após envio seu trabalho irá passar pelo proxesso de configuração das execuções e após 15, podendo o tempo ser menor, estará concluído:

![015](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/38bcb406-4864-4789-b399-99a9ea7ae479)

Pipeline com as etapas do processo de aprendizado e os testes realizados
![17](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/f4d26091-7dcb-44b0-90a3-a7a0bf6eb36a)

## Teste do modelo

Na página do modelo, cliquei na aba "Pontos de extremidade". Também é possível acessar pelo menu lateral em "Pontos de extremidade". Cliquei no ponto correspondente ao modelo gerado. Em seguida, acessei a aba "Testar".

Para o teste, utilizei o json abaixo:

``` JASON
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}
```

A previsão gerada foi: 361.95

![18](https://github.com/SamuelMckensy/DIO-Microsoft-Azure-AI-Fundamentals/assets/138621764/54a88d6d-13d1-4148-8169-d14d28ae7801)




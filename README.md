# DIO - .NET Trail - API and Entity Framework
[Digital Innovation One](https://www.dio.me/?ref=RE6NDV822B)

## Design challenge

For this challenge, I needed to use his knowledge acquired in the series of studies on API and Entity Framework, from DIO's .NET track.

## Context
I needed to build a task manager system, where you can register a list of tasks that will allow you to better organize a routine.

This task list needs to have a CRUD, that is, it should allow you to get the records, create, save and delete these records.

I had the option of creating the application as a Web API or MVC type, I chose Web API.


![Diagrama da classe Tarefa](diagrama.png)

The migration to update the database was generated.

## Methods
The methods were created according to the example below:


**Swagger**


![Métodos Swagger](swagger.png)


**Endpoints**


| Verbo  | Endpoint                | Parâmetro | Body          |
|--------|-------------------------|-----------|---------------|
| GET    | /Tarefa/{id}            | id        | N/A           |
| PUT    | /Tarefa/{id}            | id        | Schema Tarefa |
| DELETE | /Tarefa/{id}            | id        | N/A           |
| GET    | /Tarefa/ObterTodos      | N/A       | N/A           |
| GET    | /Tarefa/ObterPorTitulo  | titulo    | N/A           |
| GET    | /Tarefa/ObterPorData    | data      | N/A           |
| GET    | /Tarefa/ObterPorStatus  | status    | N/A           |
| POST   | /Tarefa                 | N/A       | Schema Tarefa |

This is the Task schema (model), used to pass to methods that require:

```json
{
  "id": 0,
  "titulo": "string",
  "descricao": "string",
  "data": "2022-06-08T01:31:07.056Z",
  "status": "Pendente"
}
```


## Solution
The code was in half, I continued obeying the rules described above, so that we have a functional program.

 [Certificate: 📜](https://www.dio.me/certificate/E947132F/share)

# apptodo
Meus estudos em python, fazendo uma aplicação estilo app To-Do

1. Estrutura Básica - A Classe TodoApp
class TodoApp: - Cria uma "classe" que é como um molde para o app
def __init__(self): - Método especial que roda quando crio um novo app
self.tarefas = [] - Cria uma lista VAZIA onde vai guardar as tarefas

2. Adicionando Tarefas
self.tarefas.append() - Adiciona um item na lista de tarefas
{"tarefa": tarefa, "concluida": False} - Cria um "dicionário" com:
  "tarefa": o texto da tarefa (ex: "Estudar")
  "concluida": False - Começa como NÃO concluída
print(f"Tarefa '{tarefa}' adicionada!") - Mostra mensagem de confirmação

3. Listando Tarefas
if not self.tarefas: - Verifica se a lista está VAZIA
enumerate(self.tarefas, 1) - Percorre a lista criando números (1, 2, 3...)
status = "✓" if tarefa["concluida"] else " " - Se concluída mostra ✓, senão espaço vazio
print(f"{i}. [{status}] {tarefa['tarefa']}") - Formata bonitinho: 1. [✓] Estudar

4. Marcar como Concluída
self.tarefas[numero-1] - Acessa a tarefa pelo número (subtrai 1 porque listas começam em 0)
["concluida"] = True - Muda o status para True (verdadeiro)
try/except - Tenta executar, se der erro (número inválido) mostra mensagem

5. Remover Tarefas
self.tarefas.pop(numero-1) - Remove a tarefa da lista e guarda ela em tarefa_removida
Mostra qual tarefa foi removida


# Comandos Básicos - Terminal
```
const accounts = await web3.eth.getAccounts()

accounts

accounts[0]
```

# Comando Básicos do Contrato - Terminal
```
const taskManager = await TaskManager.deployed()

taskManager. [TAB] [TAB]

taskManager.nTasks()

(await taskManager.nTasks()).toString()

taskManager.listMyTasks()

taskManager.getTask(0)

taskManager.getTask(1)

tx = await taskManager.addTask("Study Solidity", 1, 2, {from: accounts[1]})

tx.logs[0]

taskManager.listMyTasks({from: accounts[1]})

taskManager.getTask(2, {from: accounts[1]})

taskManager.updatePhase(1, 2)

taskManager.getTask(1)
```
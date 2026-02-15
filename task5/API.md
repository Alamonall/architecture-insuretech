# Запросы

1. Получение клиента
2. Получение документов клиента
3. Получение родственников клиента

# Сущности

1. Клиент
2. Документы
3. Родственники

# GraphQL-версия API

query {
  client(id) {
    id
    name
    age
    documents {
      id
      type
      number
      issueDate
      expiryDate
    }
    relatives {
      id
      relationType:
      name
      age
    }
  }
}

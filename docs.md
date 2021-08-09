```
1.  main.ts - bootstrap the server with MessagesModule

    Allow usage of global pipes (ValidationPipe), so CreateMessageDto 
    is passed to controller @Post() in order to validate the incoming request body

    *DTO - Data Transfer Object
```

```
2.  messages.module.ts - MessagesModule manifests MessageController and 
    DI Providers MessagesRepository, MessagesService

    *DI - Dependency Injection. Provides a container for single instances that are reused trough
    the module.
    *IOC - Inversion Of Control. Provides specific instances services, repositories etc. to some 
    APIs consumers

    MessagesRepository simulates db while writing and reading from json file.
    MessagesService consumes the MessagesRepository interface and provides methods for interaction.
```

```
3.  messages.controller.ts - MessageController resolves rest endpoints at 'messages' base url
```

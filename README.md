# Whatsapp Web Clone

The idea to create WhatsApp Web Clone is to somply use
- JS Tabs Project
  - For viewing the different chats from different users
- Array of chats
  - So that we can simply pus hthe new messages into the <br></br>
    ```javascript
    let messages = [
        {
            sender: (true/false),
            messages: "lorem ipsum"
        },
    ];
    ```

We will use one single array comprising of different objects, which is updates when the page reloads. <br>
**REASON**: Since thi is just a frontend projct I just need to develop something that will show the basic features of WhatsApp.

```javascript
let rohil: [
    contacts: [
        "Mark",
        "Thomas",
        "Jack",
        "Walter",
    ],
    chats: [
        "Mark": [
            {
                sender: (true/false),
                message: "lorem ipsum"
            }
        ],
        "Thomas": [
            {
                sender: (true/false),
                message: "lorem ipsum"
            }
        ],
        "Jack": [
            {
                sender: (true/false),
                message: "lorem ipsum"
            }
        ],
        "Walter": [
            {
                sender: (true/false),
                message: "lorem ipsum"
            }
        ],
    ]
]
```

Though the original idea is o update when the page reloads that woukld mean we need another set couter variable to store it for all the chats that are there and then lastly append it. That would require more space. Thus we have to append the messages and settings on the go and store all this in the `LocalStorage` and go give the effect of stored WhatsApp chats in the database.

- **Message Deletion** <br>
  To delete messages instead of deleting them, updating feels more appropriate, since this is just a front-end

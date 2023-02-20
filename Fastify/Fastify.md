# Basic setup

```javascript
let items = ["1 ", "2", 3]


const PORT = 5000
const fastify = require("fastify")({logger: true})

fastify.get("/items", (req, res) => {
    res.send({test: "hello"})
})

const start = async () => {
    try {
        await fastify.listen(PORT)
    } catch (error) {
        fastify.log.error(error)
        process.exit(1)
    }
}
start()

```

# With Items

```javascript
let items = ["1 ", "2", 3]

const PORT = 5000
const fastify = require("fastify")({logger: true})

fastify.get("/items", (req, res) => {
    res.send(items)
})

const start = async () => {
    try {
        await fastify.listen(PORT)
    } catch (error) {
        fastify.log.error(error)
        process.exit(1)
    }
}
start()

```

# Get single item

```javascript
let items = ["1 ", "2", 3]

const PORT = 5000
const fastify = require("fastify")({logger: true})

fastify.get("/items/:id", (req, res) => {
    const {id} = req.params
    const item = items.find((item) => item.id === id)

    res.send(item)
})

const start = async () => {
    try {
        await fastify.listen(PORT)
    } catch (error) {
        fastify.log.error(error)
        process.exit(1)
    }
}
start()

```

# Export Routes

```javascript
const items = require('/../items')

function itemRoutes(fastify, options, done) {


    fastify.get("/items/:id", (req, res) => {
        const {id} = req.params
        const item = items.find((item) => item.id === id)

        res.send(item)
    })

    done()
}

module.export = itemRoutes
_______________________________________

fastify.register(require('./routes/items'))

```

# Validation Schema

```javascript
const getItems = {
    schema: {
        res: {
            200: {
                type: "array",
                items: {
                    type: "object",
                    properties: {
                        id: {type: "string"},
                        name: {type: "string"}
                    }
                }
            }
        }
    }
}

fastify.get("/items/:id", getItems(req, res)
=>
{
    reply.send(items)
}
)
```

# PropI

```javascript
const Items = {
    type: "array",
    items: {
        type: "object",
        properties: {
            id: {type: "string"},
            name: {type: "string"}
        }}}

const getItems = {
    schema: {
        res: {
            200: Items
                // type: "array",
                // items: {
                //     type: "object",
                //     properties: {
                //         id: {type : "string"},
                //         name: {type : "string"}
            }}}
```

# Moving handler up

```javascript
const Items = {
    type: "array",
    items: {
        type: "object",
        properties: {
            id: {type: "string"},
            name: {type: "string"}
        }}}

const getItems = {
    schema: {
        res: {
            200: Items
        }
    },
    handler: function (req, res) {
            const {id } =req.params
            const item = items.find((item) => item.id === id)
            res.send(item)
    }
}

const items = require('/../items')

function itemRoutes(fastify, options, done) {

 // fastify.get("/items/:id", getItems, (req, res) => {
 //     const {id } =req.params
 //     const item = items.find((item) => item.id === id)
 //     res.send(item)
    done()
}

module.export = itemRoutes

```

# Controller Group

```javascript
const items = require('.../Items')

const getItems = (req, res) => {
    res.send(items)
}

const getItem = (req, res) => {
    const {id} = req.params
    const item = items.find((item) => item.id === id)
    res.send(item)
}

module .exports = {
    getItems, getItem
}

```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```

#

```javascript


```


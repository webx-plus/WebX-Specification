# Browser development
So you want to make a browser for WebX?\
Thats great! more competition means better browsers for everyone.\
There are some guidelines tho, see them in the document below.

## Non standard features
Sometimes browsers want to add things not in the spec.\
This is fine, there are some rules tho:
- No adding arbitrary web features to WebX (aka use any css syntax or normal html).
- Naming of features need to be aproved by the [WXWG](../wxwg.md).
- Prefixing, you must prefix the features, more info in the prefixing section

## Prefixing
Prefixed features must appear in the [browser.api](../lua/v2/globals/browser.md) in the lua v2 api as follows:
```lua
browser.api._{name}_{feature}
```
where:
- name - is the [browser.agent](../lua/v2/globals/browser.md)
- feature - the name of the fature (we_use_this_type_of_naming)

Prefix feature use.\
Lets say you add `delete_system32` api inside browser\
Then it should look like:
```lua
browser._{name}_delete_system32()
```

## Choosing a lua engine
Which lua engine to use?\
Well there it depends on use case and language.\
Below are some recomendations based on current browsers.

|       | Fast    | Small   | Integrated | Async   |
| JS    | Wasmoon | Fengari | Fengari    | Wasmoon |
| Other | Luau    | Luau    | Luau       | Luau    |
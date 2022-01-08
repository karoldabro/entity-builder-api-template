# Entity builder API template
Template for [Entity builder](https://github.com/GooGee/Entity-Builder) that creates API files.
## Features
1. API controller:
    - create
    - show
    - list
    - update
    - destroy
2. Model with uuid as a primary key
3. Factory
4. Migration
5. Repository
6. Resource
7. Store and update requests
8. API test
## Usage
### Entity builder
1. [Start Entity builder](https://github.com/GooGee/Entity-Builder#project-setup)
2. Open localhost:8080
3. Upload ApiTemplate.json from this repository
4. Start builing your API
### Generate swagger documentation
Run command:
```shell
vendor/bin/openapi
```
## Notes
- You have to implement Repository class by yourself.
- While developing package is good to use orchestra/testbench with registered sanctum provider.
- Those dependencies are required(I don't put versions):
```json
"require": {
    "dyrynda/laravel-model-uuid",
    "laravel/sanctum",
},
"require-dev": {
    "orchestra/testbench",
    "darkaonline/l5-swagger",
},
```
## TODO
- improve swagger documentation 
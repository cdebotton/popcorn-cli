# popcorn

A modular utility for scaffolding sick ass web sites and applications in the KRIP stack.

## Commands

### Initializers
- `popcorn init <name>`: Initialize a new project.
  - `--db=postgres|mysql|mariadb|sqlite`: Database engine.
  - `--dependencies=react,react-router,momentjs`: Name npm dependencies.
  - `--devDependencies=gulp,pruno`: Name npm devDependencies.
  - `--cms=cmyk|craft|wordpress|none`: Name CMS to use.

### Build tools
- `popcorn build`: Build production environment.
- `popcorn watch`: Watch site for changes during development, spin of dev server.
- `popcorn tinker`: Load application environment in your cli and work with models.
- `popcorn serve`: Serve production environment,

### Generators
- `popcorn new actions <actionCreatorName> [...actions]`: Generate a new Action Creator.
- `popcorn new store <storeName> [...actions]`: Generate a new Store.
  - `--state=propName:"InitialValue",prop2Name:null`: List properties and default values of Store state.
- `popcorn new component <componentName> [...mixins]`: Generate a new Component.
- `popcorn new model <modelName>`: Generate a new Model.
  - `--fields=fieldName:string,fieldName2:number`: List default properties and values of model.
- `popcorn new migration <tableName>`: Generate a new migration file.
  - `--fields=fieldName:string,fieldName2:number`: List default properties and values for migration.
- `popcorn new controller <resource>`: Generate a new API controller.
  - `-- actions=get,post,put,delete`: List available http actions for controller.

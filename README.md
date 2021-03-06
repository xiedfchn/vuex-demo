# Vuex Demo
Vuex is a state management pattern + library for Vue.js applications. It serves as a centralized store for all the components in an application, with rules ensuring that the state can only be mutated in a predictable fashion.
## Problems solved
- Multiple views may depend on the same piece of state.
- Actions from different views may need to mutate the same piece of state

## Core Concepts
### State
Vuex uses a single state tree - that is, this single object contains all your application level state 

### Getters
Sometimes we may need to compute derived state based on store state, for example filtering through a list of items and counting them
### Mutations
The only way to actually change state in a Vuex store is by committing a mutation.
### Actions
Actions are similar to mutations, the differences being that:
- Instead of mutating the state, actions commit mutations.
- Actions can contain arbitrary asynchronous operations.
### Modules
Due to using a single state tree, all states of our application are contained inside one big object. However, as our application grows in scale, the store can get really bloated.

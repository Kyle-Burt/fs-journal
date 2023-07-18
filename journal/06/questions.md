# Single Page Applications with Vue
/01. What is the entrypoint of an application?

  > | Main.js |

/02. What is the difference between a vue `component` and `page`?

  > | Nothing really they are both components, one can just have reusable functions |

/03. What is ***Component-Based Architecture***?

  > | the building around functions that can be used across the whole build |

/04. What are the three tags that make up a Vue component?

  > | Template, script, style |

/05. What are ***lifecycle hooks***? What are lifecycle hooks used for?

  > | functions like onmount, to run functions after they have initialized  |

/06. Which component in Vue does the vue-router use to mount pages onto?

  > | Router-view |

/07. What is the difference between the `AppState` and the state object within a component?

  > | appstate is global, state object is local |

/08. What is the responsibility of `Services` in our Vue projects?

  > | Same as in the MVC formula to run functions and change values that users don't have access to. |

/09. What are ***props*** and how are they used? Provide an example

  > | props are a way to pass data from a parent to a child component 
        defineProps({ greetingMessage: String})
        <span>{{ greetingMessage }}</span>
        <MyComponent greeting-message="hello" />
  |

/10. What is the Vue method used to create watchable objects such as `state` or `AppState`?

  > | watch() |

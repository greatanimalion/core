# app的结构
```js
 const AppContext={
    app: null as any,
    config: {
      isNativeTag: NO,
      performance: false,
      globalProperties: {},
      optionMergeStrategies: {},
      errorHandler: undefined,
      warnHandler: undefined,
      compilerOptions: {},
    },
    mixins: [],
    components: {},
    directives: {},
    provides: Object.create(null),
    optionsCache: new WeakMap(),
    propsCache: new WeakMap(),
    emitsCache: new WeakMap(),
 }

 const app={
      _uid: uid++,
      _component: rootComponent as ConcreteComponent,
      _props: rootProps,
      _container: null,
      _context: AppContext,//与AppContext关联
      _instance: null,
      version,
      get config()
      use()
      mixin()
      component()
      directive()
      mount()
      onUnmount()
      unmount()
      provide()
      runWithContext()
 }
```
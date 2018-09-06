React Redux Types
==================

# Why?
* This is a temporary fix for typing issues with react-redux as seen in this
[thread](https://github.com/DefinitelyTyped/DefinitelyTyped/pull/27724#issuecomment-418900310)
* It simply changes:
```
export interface ProviderProps<A extends Action = AnyAction> {
    /**
     * The single Redux store in your application.
     */
    store: Store<any, A>;
}
```
to this
```
export interface ProviderProps<A extends Action = AnyAction> {
    /**
     * The single Redux store in your application.
     */
    store: Store<any>;
}
```

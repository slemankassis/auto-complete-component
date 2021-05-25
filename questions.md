# Part 2 - Responses

1. PureComponent handles the shouldComponentUpdate method automatically. When props or state changes, PureComponent will do a special comparison called shallowon between props and state. Component on the other hand won’t compare current props and state to next out of the box. Thus, the component will re-render by default whenever shouldComponentUpdate is called.

    The definition of Pure Component says that for specific input parameters, we always have a specific output. The output is solely dependent on Input parameters and no other external variable. Pure Components restricts Re-Rendering.

    Example: Use PureComponent for a TextInput.

3. handleEvent methods / callbacks passed as a prop to the children. Dispatching an action using Flux/ Redux.  Using React's Context API.

4. Using shouldComponentUpdate or useMemo hook.

5. React.Fragment allows us to return an array of DOM Elements instead of only one.
Fragments is a type of doing microservices of frontend that allows rendering in same page things of other repositories at the same time. Is different from having UI components from libraries.

6. Using authentication or authorization HOC. Using i18n HOC. Using HOC for inject vars client-side to the server-side or vice versa. Add wrappers of props.

7. Handling exceptions in promises:  Will move the state of the promise to rejected or not resolved and the request failed. Callbacks: is not called always. .async...await: async keyword implicitly creates a Promise for its function.

8. setState has 2 parameters: the change of the state and an optional callback, it will be called after setting the state and it is perfect if you need to do something with the new state. setState() does not immediately mutate this.state but creates a pending state transition. Accessing this.state after calling this method can potentially return the existing value. There is no guarantee of synchronous operation of calls to setState and calls may be batched for performance gains.

9. Change class/ React.Component for const/ funcion. Remove all "this.", remove all the blind calls. replace elements of the state for useState in the following way: `const [<name of variable>, <name of setter method>] = useState(<initial value>)`. Create refs with useRef hook. Remove render method, only left `return`. Replace componentDidMount componentDidUpdate componentWillUnmount with useEffect.

10. Inline styles using the attr `style` with an object. Classnames with styles and using SCSS files. Styled components, Marial UI. Use the SCSS like an object of styles and use the styles with the `className={style_file['<className>']}`.

11. dangerouslySetInnerHTML method of React or with libs like react-html-parser. I recommend using sanitize-html npm lib in order to allow some tags only.
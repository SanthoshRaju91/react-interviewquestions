Hi, this is repository providing with a series of commonly asked interview questions with regards to React framework. 

Since the framework has got a lot of traction and popularity, the interviewers have started asking questions about a more abstract layer of Javascript. So I have consolidated some of the commonly asked questions which can be a helpful for Job seekers during their preparations.

#### Request to all the members who are viewing this, if you find any mistake or want ot contribute to improving the list of questions right here. Please raise a pull request so I can merge it. This document will be updated going forward with more questions as and when we gather more questions from our sources.

### Also a very humble request, please help me in sharing this with everyone you know can benefit. 

### My intention is to have the knowledge reachable.


## Questions
<br/>

1. Which life-cycle method is most suitable to fetch Ajax data to be rendered in the component ?
   <br/>

   > `componentDidMount()`. According to the docs, `componentDidMount()` life-cycle method is invoked immediately after a component is mounted. Intialization that requires DOM nodes should go here. [read more here](https://reactjs.org/docs/react-component.html#componentdidmount)

<br/>

2. Which type of Components can be shallow-rendered ?
   <br/>
   
   > All Components (function & class components) [read more about shallow-rendering](https://reactjs.org/docs/shallow-renderer.html)   

<br/>

3. Which inline style cannot be applied to React components ?  
   <br/>
   > Media queries

<br/>

4. You have a component which gets repeated in a list many times, and you are worried about performance. You have ensured that you use immutable data structures for your props, and you are comfortable that you always want the component's representation in the DOM to stay untouched while the prop references stay the same. How do you ensure this behavior?
    <br/>
 
    > Extend your component from React.PureComponent, this way React will only render when the prop references are updated.

<br/>

5. Which life cycle method can be used to clean up any event listeners before a component gets removed from the DOM?
    <br/>

    > componentWillUnmount() [read more about componentWillUnmount](https://reactjs.org/docs/react-component.html)

<br/>

6. What's a higher order component?
    <br/>

    > A function that takes an existing component and returns another component that wraps it.

<br/>

7. Which of the following is a valid way to hide an element based on a boolean called isVisible?
    <br/>

    > `{isVisible && <MyElement/>}` where the `isVisible` can be boolean state or a variable which toggles.

<br/>

8. Which of the following lifecycle methods does not get triggered on the component's initial render?
    <br/>

    > componentWillReceiveProps()  [read more about componentWillUnmount](https://reactjs.org/docs/react-component.html)

<br/>

9. What is wrong with this React component?
    ```javascript
    const Greeting = (props) => {
        return (
            <div>{this.state.greeting}</div>
        );
    };
    ```
    <br/>

    > State isn't supported in stateless functional components

<br/>

10. You have a css class name stored in varable cssClassName and you want to give an element that class in addition to the class "text-success". Which of the following is valid?
    <br/>

    > `<div className={`${cssClassName} text-success`}></div>`

<br/>

11. How can you retain a reference to a component that was created through JSX, so that you can interact with it programmatically?
    <br/>

    > By using the ref attribute

<br/>

12. How do you generate a correct production build for React?
    <br/>

    > By making sure to pass NODE_ENV is seen as "production" while building.

<br/>

13. In your component you have a controlled input, with its value coming from state and being updated on state when the user changes the input value. You want it to have a default value which can be changed by the user, what do you need to do?
    <br/>

    > Use the defaultValue attribute, it will ensure that the value has a default but can still be overriden

<br/>

14. Can the top-level parent component also subscribe to a partial state out of the state container?
    <br/>

    > Yes. Every component should only subscribe to the elements it needs.

<br/>

15. How can you run code immediately after state has changed?
    <br/>

    > Pass a function to setState

<br/>

16.  Since props are immutable, how do you traditionally change the value passed down to a child component?
    <br/>

    > Call a function passed via props

<br/>

17. What is a good indicator that you're using the correct React production build?
    <br/>

    > No warning from React about it. And the react dev tools chrome extension, will automatically indicate when your application is using a older version of React or if your application is not production build. 

    [You can find the React Dev tool chrome extension here](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en)

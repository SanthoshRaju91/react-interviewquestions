Hi, this is repository providing with a series of commonly asked interview questions with regards to React framework. 

Since the framework has got a lot of traction and popularity, the interviewers have started asking about a more abstract layer of Javascript. So I have consolidated some of the commonly asked questions which can be a helpful place for Job seekers during their preparations.

#### Request to all the members who are viewing this, if you find any mistake or contribute to improving the list of questions right here. Please raise a pull request so I can merge it.


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
